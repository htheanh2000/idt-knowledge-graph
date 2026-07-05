---
tags: [chapter-6, part2, supply-chain, e-procurement, value-chain, logistics, RFID, B2B]
aliases: [Quản trị chuỗi cung ứng số, Digital Supply Chain Management, IDT Chapter 6]
---
# Chapter 6 - Digital Supply Chain Management

## Tổng quan (Overview)

Chương 6 mở đầu Part 2 với ứng dụng đầu tiên của digital business: [[Supply Chain Management]] (quản trị chuỗi cung ứng). Đây là khái niệm hợp nhất vì nó bao gồm cả [[Buy-side E-commerce]] (mua vào) lẫn [[Sell-side E-commerce]] (bán ra). SCM về bản chất là tối ưu hóa dòng vật chất (material flows) và dòng thông tin (information flows) liên quan đến vận hành của tổ chức. Các biến động gần đây (COVID-19, yêu cầu bền vững qua "circular economy", bất ổn thị trường) buộc chuỗi cung ứng phải resilient hơn; riêng xử lý hàng trả lại từ e-commerce đã là thách thức lớn — tỷ lệ trả hàng quần áo nữ lên tới 23% (Signifyd, 2023), và chi phí xử lý một sản phẩm trả về có thể gấp đôi, gấp ba chi phí giao đi (giao một chiếc áo khoác tốn £3–£10).

Chương trình bày các khung phân tích kinh điển: [[Value Chain]] của Porter (cùng virtual value chain, [[Value Stream]] và [[Value Network]]), phổ lựa chọn tái cấu trúc từ [[Vertical Integration]] đến [[Virtual Integration]], và vai trò công nghệ ([[EDI]], XML, [[RFID]], [[IoT]], [[ERP]]) trong việc chia sẻ thông tin giữa các đối tác. Nửa sau chương tập trung vào [[e-Procurement]]: quy trình mua sắm, các loại hình, driver, ước tính tiết kiệm chi phí, rào cản và [[B2B Marketplace]].

Bối cảnh mới của chương là "Industry 4.0" / "Logistics 4.0" — làn sóng số hóa chuỗi cung ứng bằng AI, robots, blockchain và cyber physical systems (CPS), hướng tới chuỗi cung ứng tự hành (autonomous supply chain) chống chịu tốt hơn với gián đoạn.

---

## What is Supply Chain Management? (Quản trị chuỗi cung ứng là gì)

### Định nghĩa (Definition)
[[Supply Chain Management]] (SCM) là sự phối hợp tất cả hoạt động cung ứng của một tổ chức, từ nhà cung cấp đến việc giao sản phẩm/dịch vụ cho khách hàng. Phân biệt hai nửa:
- **Upstream supply chain** (chuỗi cung ứng thượng nguồn): hoạt động với nhà cung cấp — tương đương [[Buy-side E-commerce]] (procurement + inbound logistics).
- **Downstream supply chain** (chuỗi cung ứng hạ nguồn): hoạt động phân phối tới khách hàng — tương đương [[Sell-side E-commerce]] (sales, outbound logistics, fulfilment).

### Giải thích chi tiết
- Chuỗi cung ứng không chỉ gồm supplier–buyer mà cả trung gian nhiều tầng (first-tier, second-tier suppliers/customers). Vì mỗi công ty có nhiều chuỗi cho nhiều sản phẩm, thuật ngữ chính xác hơn là **supply chain network**.
- Nhìn từ góc độ hệ thống: inputs (acquisition of resources) → process (transformation) → outputs (products/services); ranh giới hệ thống của SCM vượt ra ngoài tổ chức.
- **Quy mô vấn đề tồn kho**: theo US Department of Commerce (12/2022), $2.475.000 triệu (~$2,475 tỷ) tồn kho trên toàn bộ các loại hình doanh nghiệp Mỹ; tỷ lệ inventory/sales: Manufacturers 1,49 — Retailers 1,26 — Merchant wholesalers 1,36. **Inventory turnover** (vòng quay tồn kho = COGS / tồn kho bình quân) là thước đo hiệu quả then chốt.
- **4 trụ cột thành công của chuỗi cung ứng** (IGD, 2017): (1) Customer centric; (2) Powered by people; (3) Transformed by technology; (4) Resilient and responsive.
- [[Efficient Consumer Response]] (ECR): phát triển từ ngành bán lẻ thực phẩm Mỹ, chuyển trọng tâm từ bổ sung hàng hiệu quả (replenishment) sang **demand management** — tạo và thỏa mãn nhu cầu qua tối ưu assortment, promotion và ra mắt sản phẩm mới.
- [[Vendor-Managed Inventory]] (VMI): chuyển nhiệm vụ quản lý tồn kho, mua hàng, theo dõi đơn hàng hằng ngày từ khách hàng sang **nhà cung cấp**.
- **Industry 4.0** (McKinsey, 2022) — 4 nhóm công nghệ disruptive: (1) connectivity/data/computational power (cloud, Internet, [[Blockchain]], sensors); (2) analytics & intelligence (advanced analytics, ML, [[Artificial Intelligence|AI]]); (3) human–machine interaction (VR/AR, robotics, autonomous guided vehicles); (4) advanced engineering (3D printing, năng lượng tái tạo). Chuỗi 4 cuộc cách mạng công nghiệp: 1784 (máy hơi nước) → 1870 (điện, sản xuất hàng loạt) → 1969 (điện tử, IT, tự động hóa) → 2014 (4IR: số hóa chuỗi cung ứng, AI, RFID sensors).
- **Cyber physical system (CPS)**: nền tảng cho autonomous supply chains; IDC (2023) ghi nhận 72% supplier từng gặp gián đoạn chuỗi cung ứng mà thiếu visibility để phản ứng nhanh.
- Lợi ích số hóa (IDC 2023, % cải thiện đáng kể/tổng): chia sẻ product catalogue 42%/84%, giá 44%/82%, chứng từ hải quan 49%/80%, hóa đơn 42%/78%, đơn mua 43%/79%, thông báo giao hàng 44%/84%.

### Ví dụ thực tế
[[Case 6.1 Zara]]: Zara dùng [[Vertical Integration]] + JIT + dữ liệu thời gian thực để đưa sản phẩm từ concept đến cửa hàng trong 15 ngày (chuẩn ngành: 6 tháng), bán 85% hàng nguyên giá so với 60–70% trung bình ngành. Nike tăng operating margin 10–15%/năm trong 4 năm liên tiếp nhờ cải tiến chuỗi cung ứng (AMR, 2008).

### Liên kết
- [[Supply Chain Management]], [[Vendor-Managed Inventory]], [[Efficient Consumer Response]], [[Industry 4.0]], [[Buy-side E-commerce]], [[Sell-side E-commerce]]

---

## What is Logistics? (Logistics là gì)

### Định nghĩa (Definition)
[[Logistics]] là "time-related positioning of resource" (định vị nguồn lực theo thời gian) — đảm bảo hàng hóa/dịch vụ theo "five rights": đúng nơi, đúng lúc, đúng số lượng, đúng chất lượng, đúng giá (Chartered Institute of Logistics and Transport).

### Giải thích chi tiết
- Thực tế logistics thường chỉ **inbound logistics** (nhận nguyên liệu vào) và **outbound logistics** (giao sản phẩm ra).
- **"Last mile"** ngày càng quan trọng do tỷ trọng bán lẻ online tăng: same-day/next-day delivery, Amazon lockers, nhận hàng tại cửa hàng tiện lợi.
- 4 điều kiện tiên quyết cho same-day delivery (Hausmann et al., 2014; McKinsey 2020): (1) sản phẩm sẵn có tại địa phương; (2) real-time overview về tồn kho; (3) picking & packing nhanh; (4) linh hoạt pick-up/giao nhiều lần trong ngày (geofencing, dynamic rerouting).
- Amazon: riêng việc **có** lựa chọn same-day delivery đã tăng purchase conversion khi checkout thêm 20–30%, dù ít khách thực sự chọn.

### Liên kết
- [[Logistics]], [[Omnichannel]], Fulfilment

---

## Push and Pull Supply Chain Models (Mô hình đẩy và kéo)

### Định nghĩa (Definition)
[[Push Supply Chain]]: nhà sản xuất phát triển sản phẩm, xác định thị trường, tạo kênh phân phối để **đẩy** sản phẩm ra thị trường — tối ưu cho chi phí sản xuất. [[Pull Supply Chain]]: xuất phát từ **nhu cầu khách hàng**, hợp tác chặt với khách hàng và nhà cung cấp trong phát triển sản phẩm — tối ưu cho customer response.

### Giải thích chi tiết
- Chuyển dịch tư duy từ push → pull (hoặc kết hợp push–pull) nhất quán với ECR và tư duy value chain.
- Mô hình pull đòi hỏi liên kết chặt giữa các mắt xích qua công nghệ ([[EDI]]) để giảm chuyển giao chứng từ và nhập liệu lại.

### Liên kết
- [[Push Supply Chain]], [[Pull Supply Chain]], [[Efficient Consumer Response]], [[EDI]]

---

## The Value Chain (Chuỗi giá trị)

### Định nghĩa (Definition)
[[Value Chain]] (Porter, 1980) là mô hình mô tả các hoạt động gia tăng giá trị nối cung với cầu của công ty: **primary activities** (đóng góp trực tiếp đưa hàng đến khách) và **support activities** (hạ tầng, IS, nhân sự). Công thức: Value = (Benefit của từng hoạt động VC − chi phí) + (Benefit của từng interface giữa các hoạt động − chi phí).

### Giải thích chi tiết
- **Virtual value chain** (Rayport & Sviokla, 1996): chuỗi giá trị ảo song song với chuỗi vật lý — Internet tạo giá trị bằng gathering, organising, selecting, synthesising, distributing thông tin.
- **Điểm yếu của mô hình VC truyền thống**: thiên về sản xuất vật chất, một chiều (push), không nhấn mạnh value networks. Mô hình sửa đổi của Deise et al. (2000) bắt đầu từ **market research** — nhấn mạnh environmental scanning thời gian thực, rút ngắn time-to-market.
- **[[Value Stream]]** (Womack & Jones, 1998): tập hợp hành động qua 3 nhiệm vụ quản lý — (1) problem-solving (phát triển sản phẩm mới); (2) information management (nhận đơn → giao hàng); (3) physical transformation (nguyên liệu → thành phẩm). Value stream analysis phân loại hoạt động: tạo giá trị / không tạo giá trị nhưng bắt buộc / không tạo giá trị → loại bỏ ngay. Ví dụ lon cola: tổng cycle time gần **1 năm** từ mỏ bauxite đến nhà, trong khi thời gian xử lý thực chỉ ~3 giờ.
- **Value chain analysis** — quy trình 5 bước của Porter & Millar (1985): (1) đánh giá information intensity; (2) xác định vai trò IS trong cấu trúc ngành; (3) xếp hạng cách IS tạo lợi thế cạnh tranh; (4) khám phá IS có thể sinh ra business mới; (5) lập kế hoạch business-driven.
- **[[Value Network]]**: khi outsourcing tăng, quản lý liên kết với đối tác trở nên then chốt; gồm supply-side partners, đối tác thực hiện core VC activities, sell-side partners và **value chain integrators**. Mạng lưới có tính động — thêm/bớt đối tác theo điều kiện thị trường.
- Ví dụ hiệu quả: BT triển khai e-procurement đạt 95% mua sắm online cho văn phòng phẩm, giảm chi phí giao dịch mua trung bình từ **£56 xuống £40** (IBF, 2008). Tesco Information Exchange giúp giảm tồn kho RDC/in-store xuống còn 2–3 ngày, bổ sung hàng liên tục trong 24 giờ; Tesco Exchange (2022) cho 3.500+ supplier bán/tặng hàng dư thừa cho nhau.

### Ví dụ thực tế
Dell: outsourcing không phải để "vứt bỏ quy trình không tạo giá trị" mà để "phối hợp hoạt động tạo giá trị tối đa cho khách hàng" — build-to-order và giao trong 24 giờ ("Smart Selection").

### Liên kết
- [[Value Chain]], [[Value Stream]], [[Value Network]], [[Virtual Integration]], [[e-Procurement]]

---

## Options for Restructuring the Supply Chain (Tái cấu trúc chuỗi cung ứng)

### Định nghĩa (Definition)
Phổ lựa chọn quản lý chuỗi cung ứng trải từ [[Vertical Integration]] (kiểm soát nội bộ — sở hữu các khâu) qua **vertical disintegration** (supply chain disaggregation) đến [[Virtual Integration]] (kiểm soát bên ngoài qua outsourcing).

### Giải thích chi tiết
- Xu hướng nửa sau thế kỷ 20: từ vertical integration → virtual integration (ngành ô tô outsource dần đèn, nội thất, cả động cơ; marketing giao cho agency).
- **3 quyết định chiến lược** (Hayes & Wheelwright, 1994): (1) **Direction** — mở rộng upstream (defensive) hay downstream (offensive, ví dụ hãng dược mua pharmacy benefit managers để "gần khách hàng hơn"); (2) **Extent** — mức độ tích hợp (wide vs narrow process span); (3) **Balance** — mức độ các khâu phục vụ riêng chuỗi của mình.
- So sánh kinh điển: **IBM thập niên 1980s** (tự sản xuất processor, ổ cứng, case, màn hình, chuột — vertical integration) vs **Dell thập niên 1990s–2000s** (mọi linh kiện từ bên thứ ba: Intel, Seagate, Sony, Microsoft — virtual integration).
- E-commerce hỗ trợ chiến lược narrow process span bằng cách tăng dòng thông tin giữa các thành viên — nhưng đòi hỏi mọi thành viên đều e-enabled.

### Liên kết
- [[Vertical Integration]], [[Virtual Integration]], [[Outsourcing]], Virtual Organisation

---

## Using Digital Business to Restructure the Supply Chain (Dùng digital business tái cấu trúc chuỗi)

### Định nghĩa (Definition)
**Information supply chain (ISC)**: góc nhìn lấy thông tin làm trung tâm — mỗi thực thể tạo giá trị bằng cách cung cấp đúng thông tin, cho đúng đối tượng, đúng thời điểm, một cách an toàn (March et al., 2007).

### Giải thích chi tiết
- **[[Bullwhip Effect]]** (information asymmetry): khuếch đại tín hiệu nhu cầu và dao động tồn kho dọc chuỗi cung ứng; ECR và chia sẻ thông tin là cách giảm thiểu, nhưng bị cản bởi thiếu chuẩn, chi phí, mức độ tin cậy giữa đối tác.
- **Công nghệ và chuẩn dữ liệu** cho eSCM: [[EDI]] (trao đổi đơn hàng, phiếu giao, hóa đơn); XML/XML-EDI (truyền dữ liệu one-to-many phức tạp hơn); middleware (tích hợp/dịch yêu cầu giữa hệ thống); email/web thủ công. Dữ liệu đổ vào [[ERP]] với module material requirements planning (MRP).
- **5 lợi ích của eSCM**: (1) tăng hiệu suất từng quy trình (giảm cycle time, chi phí/đơn); (2) giảm độ phức tạp chuỗi ([[Disintermediation]] — bán trực tiếp); (3) tích hợp dữ liệu tốt hơn giữa các mắt xích; (4) giảm chi phí qua outsourcing/virtual integration; (5) đổi mới sáng tạo và customer responsiveness.
- **Upstream (IS-supported)**: procurement + upstream logistics; ví dụ Tesco Information Exchange (extranet với GE Information Services cho supplier truy cập EPOS data), Sainsbury Information Direct.
- **[[RFID]] và [[IoT]]**: thẻ RFID gắn trên sản phẩm trong kho/cửa hàng, đọc bằng radio để đánh giá tồn kho; khi reader kết nối Internet để cập nhật vị trí/trạng thái → Internet of Things. Xem [[Case 6.3 RFID]].
- **Downstream**: outbound logistics + fulfilment. Tesco.com — site tạp hóa online lớn nhất thế giới, chiến lược disintermediation giảm vai trò chi nhánh. Bài học Amazon: split shipments (giao nhiều lần cho một đơn) đội chi phí — Mỹ chiếm 86% doanh thu Amazon với mạng 7 trung tâm phân phối.
- **[[Supply Chain Visibility]]**: IS phải cho phép nhân viên, supplier, logistics provider, khách hàng truy cập thông tin chuỗi cung ứng với personalised views + bảo mật (không lộ differential pricing); kiến trúc điển hình gồm central operational database (thuộc ERP như SAP, Baan) chia thành ứng dụng **planning** và **execution**.

### Ví dụ thực tế
[[Case 6.2 Argos]]: tích hợp website với hệ thống logistics cho real-time stock availability; Click & Collect chiếm hơn nửa online sales; digital participation đạt 80% (2022).

### Liên kết
- [[Bullwhip Effect]], [[EDI]], [[ERP]], [[RFID]], [[IoT]], [[Supply Chain Visibility]], [[Disintermediation]]

---

## Supply Chain Management Implementation (Triển khai SCM)

### Định nghĩa (Definition)
Triển khai eSCM là quá trình chuẩn hóa dữ liệu, chọn chiến lược, thiết lập đo lường hiệu quả và quản lý quan hệ đối tác — trong bối cảnh "connected consumer" khiến nhiệm vụ "đúng sản phẩm, đúng khách, đúng lúc, đúng giá" phức tạp hơn cấp số nhân (KPMG, 2017).

### Giải thích chi tiết
- **Data standardisation**: rào cản lớn nhất là hệ thống không tương thích; marketplace ngành dọc như Elemica (hóa chất) thành công nhờ ít đối tác. Lợi ích chuẩn hóa (Schemm et al., 2007): quản trị đơn/mặt hàng cải thiện 50%, từ chối coupon tại quầy giảm 40%, công sức quản lý dữ liệu giảm 30%, out-of-stock giảm từ 8% → 3%.
- **Quy trình chiến lược SCM**: dùng [[SOSTAC]] (Situation–Objectives–Strategy–Tactics–Actions–Control) theo Hughes et al. (1998); 4 lựa chọn chiến lược theo **scope × speed of change** — thay đổi hẹp (cải tiến vận hành, rủi ro thấp) vs tái cấu trúc triệt để (rủi ro cao, phần thưởng lớn).
- **Đo lường hiệu quả eSCM** (Sambasivan et al., 2009) — 13 nhóm: cost, profitability (ROI), customer responsiveness, flexibility, supply chain partnership, production metrics, delivery performance, customer service, finance & logistics cost, cost performance, time performance, quality performance, CRM.
- **Managing partnerships** (Stuart & McCutcheon, 2000): "received wisdom" = focus core competencies + giảm số supplier + xây quan hệ tin cậy; nhưng lựa chọn đối tác phải theo mục tiêu — cost reduction → quan hệ cạnh tranh (arm's-length); value-added (tốc độ giao, customisation) → strategic alliance/cooperative partnership. Phổ 9 lựa chọn từ insourcing toàn phần đến outsourcing cạnh tranh.
- **Managing global distribution** (Arnold, 2000) — 7 hành động khi vào thị trường nước ngoài: tự chọn distributor; chọn người phát triển được thị trường; coi họ là đối tác dài hạn; cam kết tiền + quản lý + marketing; giữ quyền kiểm soát chiến lược marketing; yêu cầu dữ liệu thị trường/tài chính chi tiết; kết nối các distributor quốc gia sớm.
- PwC Global Supply Chain Survey (2013, 500 chuyên gia): chỉ 45% đồng ý chuỗi cung ứng được coi là tài sản chiến lược; ngành retail & consumer goods có inventory turns cao nhất ở nhóm "leaders" (18,2 lần) so với "laggards" (3,3 lần).

### Ví dụ thực tế
[[Mini 6.1 Robots AI SCM]]: robots trong kho hàng và mạng lưới AI tự thiết kế, tự chọn chuỗi cung ứng hiệu quả nhất — hướng tới autonomous supply chain.

### Liên kết
- [[SOSTAC]], [[Supply Chain Visibility]], [[Outsourcing]], Performance Management

---

## What is e-Procurement? (Mua sắm điện tử là gì)

### Định nghĩa (Definition)
[[e-Procurement]] là tích hợp điện tử toàn bộ hoạt động mua sắm: purchasing, vận chuyển, goods-in, lưu kho trước khi sử dụng. "Procurement" rộng hơn "purchasing" — bao gồm cả inbound logistics. Mục tiêu là "five rights of purchasing" (Baily et al., 1994): đúng giá, đúng thời điểm, đúng chất lượng, đúng số lượng, đúng nguồn.

### Giải thích chi tiết
- **Phân loại theo cái được mua**: production-related procurement (nguyên liệu sản xuất) vs non-production/operating procurement (văn phòng phẩm, IS, **MRO goods** — maintenance, repair, operations).
- **Phân loại theo cách mua**: systematic sourcing (hợp đồng đàm phán với supplier quen) vs spot sourcing (mua ngay hàng commodity); straight rebuy vs modified rebuy — e-procurement giúp rebuy đơn giản hơn.
- **8 loại trung gian trong e-procurement** (Riggins & Mitra, 2007): traditional manufacturers, direct sales manufacturers, value-added procurement partners, online hubs (Elemica), knowledge experts, online information services, online retailers (Euroffice, Staples), portal communities.
- **5 loại ứng dụng e-procurement** (Knudsen, 2003; Smart, 2010): (1) e-sourcing (tìm supplier mới); (2) e-tendering (RFI/RFP); (3) e-informing (thẩm định chất lượng supplier); (4) e-reverse auctions (đấu giá ngược lấy giá thấp nhất); (5) eMRO & web-based ERP (lõi giao dịch — requisition, order, nhận hàng).
- **First-generation e-procurement**: electronic procurement systems (EPS), workflow, EDI links — đã tồn tại từ lâu.

### Ví dụ thực tế
Quy trình giấy truyền thống: end-user tìm hàng → điền requisition → manager duyệt → buyer đặt hàng → nhận hàng → đối chiếu delivery note + invoice → thanh toán. E-procurement rút ngắn cycle time và loại bỏ nhập liệu trùng lặp.

### Liên kết
- [[e-Procurement]], [[EDI]], [[B2B Marketplace]], [[ERP]]

---

## Drivers, Benefits and Costs of e-Procurement (Động lực, lợi ích và chi phí)

### Định nghĩa (Definition)
Động lực chính của e-procurement là **efficiency và cost reduction** — trong nhiều trường hợp, chi phí đặt hàng vượt cả giá trị món hàng được mua.

### Giải thích chi tiết
- **5 driver** (Smart, 2010): (1) **Control** — compliance, tập trung hóa, kiểm soát ngân sách; (2) **Cost** — buying leverage qua cạnh tranh supplier, giảm chi phí giao dịch; (3) **Process** — chuẩn hóa, giảm cycle time; (4) **Individual performance** — chia sẻ tri thức, năng suất; (5) **Supplier management** — giảm số supplier, tích hợp.
- Buyer được giải phóng khỏi việc hành chính → dành thời gian cho hoạt động giá trị gia tăng (làm việc với supplier chiến lược, phân tích hành vi mua).
- **Khung Riggins & Mitra (2007)** đánh giá lợi ích theo: planning, development, inbound (trọng tâm chính — paperless + [[Vendor-Managed Inventory]]), production, outbound (liên kết đến ECR).
- **Ước tính chi phí**: Savings = Số requisitions × (chi phí cũ − chi phí mới). Số liệu Tranmit (1999): công ty vừa-lớn phát hành 1.000–5.000 requisition/tháng, chi £600.000–£3 triệu/năm cho quy trình mua sắm (chi phí median £50/item); trường hợp ngoại lệ 30.000–40.000 requisition/tháng → chi phí thường niên £18–43 triệu.
- **Tác động lợi nhuận** (Kluge, 1997): tiết kiệm lớn nhất ở công ty sản xuất — nhiều requisition giá trị thấp; ngành dịch vụ tiềm năng thấp hơn.

### Ví dụ thực tế
[[Case 6.4 Honeywell]]: tích hợp ERP (SAP) với SCM và e-procurement cho hàng trăm linh kiện điện tử vi mô đặt từ 7+ quốc gia — tăng năng suất buyer, dự báo chính xác ngày hàng về, rút ngắn order cycle, giảm tồn kho.

### Liên kết
- [[e-Procurement]], [[Vendor-Managed Inventory]], [[Efficient Consumer Response]]

---

## Barriers, Risks and Implementation (Rào cản và triển khai)

### Định nghĩa (Definition)
Rào cản e-procurement gồm cả yếu tố kỹ thuật (tích hợp hệ thống) lẫn tổ chức (văn hóa, kháng cự thay đổi, nguy cơ giảm biên chế phòng mua hàng).

### Giải thích chi tiết
- **Rào cản với supplier** (CIPS, 2008): vấn đề cạnh tranh trong collaborative purchasing; lo ngại margin giảm do e-auctions; lợi ích đàm phán bị chia sẻ với đối thủ cùng sàn; tạo catalogue tốn kém; kháng cự văn hóa.
- **CIPS khuyến nghị mạnh**: re-engineer quy trình TRƯỚC khi triển khai ePurchasing — không chỉ tự động hóa quy trình giấy hiện có.
- **Các loại hệ thống** phủ chu trình mua sắm: stock-control system; CD/web-based catalogue; email/database workflow; order entry trên website; accounting systems; integrated e-procurement/ERP.
- **Tích hợp với supplier**: 3 mô hình vị trí B2B e-commerce — sell-side, buy-side, marketplace-based. Hai lựa chọn catalogue: (a) chứa catalogue trong firewall công ty; (b) **punchout catalogue** — truy cập qua firewall đến catalogue trên site supplier/trung gian.

### Ví dụ thực tế
IFO-Basware (2012): ~50% công ty vẫn nhận invoice qua email PDF; ~50% nhận XML e-invoice qua service provider; chỉ 14% có hệ thống riêng — tự động hóa vẫn hạn chế.

### Liên kết
- [[e-Procurement]], [[ERP]], [[Change Management]]

---

## B2B Marketplaces (Sàn giao dịch B2B)

### Định nghĩa (Definition)
[[B2B Marketplace]] (marketplaces/exchanges/hubs): trung gian độc lập với buyer và supplier, thuộc hiện tượng [[Reintermediation]].

### Giải thích chi tiết
- **Taxonomy Kaplan & Sawhney (2000)** theo 2 trục: how businesses buy (systematic vs spot) × what businesses buy (manufacturing inputs vs operating resources) → 4 loại marketplace. Manufacturing-input marketplaces thường là **vertical** (thép, xây dựng, hóa chất); operating resources thường **horizontal**.
- **Reverse aggregation** (gộp sức mua từ khách hàng ngược lên supplier) vs **forward aggregation** (qua distributor truyền thống).
- **Private B2B exchanges**: "walled garden of suppliers" do một manufacturer/supplier lập, thành viên phải được duyệt (RFQ, reverse auction mở nhưng có vetting).
- **Metamediaries** (Sawhney, 1999): marketplace vượt ra ngoài procurement — ví dụ PlasticsNet cung cấp supplier evaluation, tracking, certification monitoring, auctions, catalogues.
- Sau 2000, nhiều B2B marketplace thất bại về business model; thành công tập trung ở ngành dọc như Elemica (hóa chất).

### Liên kết
- [[B2B Marketplace]], [[Reintermediation]], [[e-Procurement]]

---

## The Future of e-Procurement (Tương lai của e-procurement)

### Giải thích chi tiết
- **Software agents**: tìm kiếm supplier/sản phẩm tự động theo luật định sẵn hoặc neural networks; đánh giá supplier theo tiêu chí định lượng (giá, availability, delivery) — câu hỏi mở là đánh giá **trustworthiness** thế nào.
- **AI trong procurement** (Gartner, 2017): ML tự động thu thập, phân loại, phân tích chi tiêu để tìm tiết kiệm; **cognitive procurement advisers (CPAs)** và **virtual personal assistants (VPAs)** — VPA hướng người dùng đến đúng công cụ mua, CPA đưa khuyến nghị về supplier assessment, risk management, compliance.

### Liên kết
- [[Artificial Intelligence|AI]], [[Machine Learning]], [[e-Procurement]]

---

## Case studies trong chương
- [[Case 6.1 Zara]] — Fast-fashion dùng chuỗi cung ứng làm lợi thế cạnh tranh
- [[Case 6.2 Argos]] — eSCM cải thiện tiện lợi đa kênh cho khách hàng
- [[Case 6.3 RFID]] — RFID theo dõi hàng hóa, "barcode on steroids"
- [[Case 6.4 Honeywell]] — Tích hợp SCM + e-procurement qua ERP
- [[Mini 6.1 Robots AI SCM]] — Robots và AI biến đổi chuỗi cung ứng

## Liên kết chương
- Trước: [[CH05 - Digital Business Strategy]] (Decision 6: SCM capabilities)
- Sau: [[CH07 - Digital Marketing Strategy]] (downstream/sell-side)
- Nền tảng: [[CH01 - Introduction to Digital Business]] (buy-side vs sell-side), [[CH02 - Opportunity Analysis]] (disintermediation/reintermediation)
