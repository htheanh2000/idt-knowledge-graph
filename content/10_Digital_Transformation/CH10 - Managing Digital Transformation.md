---
tags: [chapter-10, part3, digital-transformation, change-management, growth-hacking, agile, data-governance]
aliases: [Quản trị chuyển đổi số, Managing Digital Transformation, IDT Chapter 10]
---
# Chapter 10 - Managing Digital Transformation

## Tổng quan (Overview)

Chương 10 khép lại Part 3 (Implementation) bằng chủ đề trung tâm của toàn giáo trình: [[Digital Transformation]] (chuyển đổi số) — quá trình sử dụng công nghệ số để tạo mới hoặc thay đổi quy trình kinh doanh, văn hóa và trải nghiệm khách hàng nhằm đáp ứng yêu cầu thị trường thay đổi. Đại dịch COVID-19 là chất xúc tác lớn: lưu lượng Internet tăng tới 60% ở một số quốc gia ngay sau khi bùng phát (OECD, 2020), đưa chuyển đổi số thành mệnh lệnh chiến lược cho doanh nghiệp mọi quy mô.

Chương nhấn mạnh thông điệp cốt lõi: phần quan trọng của digital transformation không phải là "digital" mà là "transformation". Doanh nghiệp cần **adapt** (thích ứng, thay đổi tổ chức) với công nghệ chứ không chỉ **adopt** (áp dụng) công nghệ. Chỉ 1/8 dự án chuyển đổi số được coi là thành công hoàn toàn (Gale, 2016), nên [[Change Management]], [[Digital Maturity]] và quản trị dữ liệu là những yếu tố quyết định.

Nội dung đi từ định nghĩa và phạm vi (sell-side, buy-side, in-side), qua framework chuyển đổi (review → strategy → resourcing → deployment → evaluation), sáu giai đoạn trưởng thành số của Solis, tới [[Growth Hacking]], [[Agile]]/[[Scrum]], phân tích dữ liệu và quản trị ([[Data Governance]], COBIT, [[Legacy Systems]]).

---

## Definitions of Digital Transformation (Định nghĩa chuyển đổi số)

### Định nghĩa (Definition)
[[Digital Transformation]] là quá trình sử dụng công nghệ số để tạo ra mới — hoặc điều chỉnh — quy trình kinh doanh, văn hóa và trải nghiệm khách hàng nhằm đáp ứng các yêu cầu kinh doanh và thị trường đang thay đổi (Salesforce). Nghiên cứu và thực tiễn chưa có cách hiểu thống nhất về khái niệm này (Morakanyane et al., 2017).

### Giải thích chi tiết
Morakanyane et al. (2017) tổng hợp bốn khái niệm then chốt khi mô tả digital transformation:

- **Characteristics (đặc điểm)**: các đặc tính hành vi gắn với tác động dài hạn — tác động nhỏ hay lớn, từ từ hay đột ngột.
- **Drivers (động lực)**: lợi nhuận và tăng trưởng doanh thu mới, sự hài lòng của khách hàng, hiệu quả vận hành, sự tiện lợi, chuẩn kỹ thuật cao, tăng business agility, năng suất nhân viên và lợi thế cạnh tranh (Ezeokoli et al., 2016). Công nghệ số là điều kiện cần nhưng phải kết hợp văn hóa, chiến lược và nhân lực am hiểu số (Kane et al., 2015).
- **Impacts (tác động)**: chia thành customer-focused và organisation-focused; mục tiêu chính là **value creation** cho cả tổ chức lẫn khách hàng.
- **Transformed areas (lĩnh vực chuyển đổi)**: Westerman (2014) xác định ba khu vực trọng tâm — customer experience, operational processes và [[Business Model]].

Phân biệt quan trọng **Adopting vs Adapting**: adopt nghĩa là đưa công nghệ vào mà tổ chức không thay đổi; adapt nghĩa là tổ chức thay đổi để tận dụng công nghệ. Global Center for Digital Business Transformation định nghĩa chuyển đổi số là "organizational change through the use of digital technologies and business models to improve performance" (Wade, 2015).

### Ví dụ thực tế
COVID-19: học trực tuyến, làm việc từ xa, doanh nghiệp chuyển sang [[Revenue Model]] số để giữ dòng doanh thu; AI được dùng nghiên cứu vaccine; ứng dụng mobile "track and trace" theo dõi dịch.

### Liên kết
- [[Digital Transformation]] · [[Digital Business]] · [[Business Model]] · [[Change Management]]

---

## The Applications Portfolio (Danh mục ứng dụng — tiền đề của chuyển đổi số)

### Định nghĩa (Definition)
[[Application Portfolio Analysis]] (Ward & Peppard, 2002) là mô hình phân loại đầu tư công nghệ theo ý nghĩa chiến lược mà tổ chức đặt vào nó. "Application" ở đây là **toàn bộ quy trình kinh doanh** chứa các thành phần IT, dữ liệu và luồng tri thức — không chỉ là phần mềm.

### Giải thích chi tiết
Bốn loại ứng dụng:

1. **High potential**: chưa có nhưng có thể có giá trị tương lai; mang tính thử nghiệm (alpha/beta), entrepreneurial; phải biết **đóng dự án đúng lúc** nếu không chứng minh được tiềm năng.
2. **Strategic**: mang lại lợi thế chiến lược; đòi hỏi cải tiến liên tục để tránh bị đối thủ sao chép; thành phần có tính "bí mật", thường phát triển nội bộ. Khi mất lợi thế → trở thành key operational hoặc support.
3. **Key operational**: nền tảng cho vận hành trong ngành, dùng để **tránh bất lợi cạnh tranh**; ví dụ AWS "san phẳng sân chơi" giữa các nhà vận hành cùng ngành — cloud computing chính là thời điểm data processing trở thành key operational application.
4. **Support**: tồn tại vì mục đích thông thường/pháp lý (ví dụ payroll); tiêu chí là giải pháp chi phí thấp nhất dài hạn, dễ outsource; Microsoft Office thắng nhờ tổng chi phí sở hữu (đào tạo, hỗ trợ) thấp dù giá gấp đôi G Suite.

Gartner hype cycle 2023 nêu bốn công nghệ mới nổi đáng chú ý (3–8 năm tới phổ cập): **neuromorphic computing**, **self-supervised learning**, [[Metaverse]] (BMW Pilot Plant Munich dùng AR headset kiểm tra chi tiết xe prototype) và **human-centred AI (HCAI)**.

### Ví dụ thực tế
BMW dùng [[Metaverse]]/AR trong nhà máy; AWS là key operational application của ngành e-commerce.

### Liên kết
- [[Application Portfolio Analysis]] · [[Hype Cycle]] · [[Metaverse]] · [[Generative AI]]

---

## The Scope of Digital Transformation (Phạm vi chuyển đổi số)

### Định nghĩa (Definition)
Chuyển đổi số có thể cách mạng hóa ba khu vực chính của doanh nghiệp: **sell-side** (marketing và e-commerce), **buy-side** ([[Supply Chain Management]] và procurement) và **in-side** (quy trình và quản trị tri thức).

### Giải thích chi tiết
**1. Sell-side**: cải thiện truyền thông marketing để thu hút khách hàng; tránh sai lầm chỉ tập trung công nghệ — bắt đầu từ customer value proposition và [[Customer Experience]]. Tabrizi et al. (2019, HBR): "nếu con người thiếu mindset thay đổi và thực hành tổ chức đang lỗi, digital transformation sẽ chỉ phóng đại những lỗi đó". [[7Ds of Digital Marketing]] (Chaffey & Ellis-Chadwick) định khung phạm vi quản trị: digital goals & strategy, audiences, devices, platforms, media, data, technology.

**2. Buy-side**: chuyển đổi số giúp chuỗi cung ứng cải thiện hiệu quả chi phí, hiệu suất vận hành–tài chính, tính hướng khách hàng và quản trị quan hệ đa nhà cung cấp (Alabdali & Salam, 2022). Stackpole (2020) nêu 5 công nghệ chuỗi cung ứng tạo lợi thế cạnh tranh: [[IoT]] (giám sát tài sản, tránh thất lạc hàng), [[Blockchain]] (track-and-trace, chống hàng giả), **AI/machine learning/analytics**, **robots và automation** (robot đóng gói của Amazon nhanh gấp 4–5 lần nhân công trung bình), **3D printing** (sản xuất phi tập trung, giảm chi phí logistics).

**3. In-side**: [[Knowledge Management]] — thu thập, lưu trữ, chia sẻ tri thức để cải thiện ra quyết định và đổi mới; gắn với Industry 4.0. Lợi ích: streamline quy trình, tăng cộng tác, quản trị dữ liệu tốt hơn, linh hoạt (remote work, cloud), cá nhân hóa trải nghiệm khách hàng.

Ba khu vực liên kết chặt — thay đổi một khu vực thường ảnh hưởng khu vực khác, nên cần **cách nhìn toàn diện (holistic)**.

### Ví dụ thực tế
[[Case 10.1 Counterfeit Drugs Africa]] (buy-side: blockchain + mobile + RFID chống thuốc giả); [[Mini 10.1 Siemens]] (in-side: nền tảng tri thức ShareNet); [[Mini 10.2 Carrefour]] (sell-side + supply chain: online sales tăng 60% năm 2020).

### Liên kết
- [[Supply Chain Management]] · [[e-Procurement]] · [[Knowledge Management]] · [[IoT]] · [[Blockchain]] · [[RFID]] · [[7Ds of Digital Marketing]]

---

## Digital Transformation Strategy (Chiến lược chuyển đổi số)

### Định nghĩa (Definition)
Digital transformation strategy là quá trình dùng công nghệ số để chuyển đổi [[Business Model]], vận hành và trải nghiệm khách hàng của tổ chức; xác định khu vực trọng tâm chuyển đổi và tận dụng công nghệ để cải thiện chúng.

### Giải thích chi tiết
Cân nhắc then chốt khi xây chiến lược: (1) xác định rõ mục tiêu, (2) đánh giá năng lực hiện tại, (3) xây roadmap, (4) engage stakeholders, (5) giám sát và điều chỉnh liên tục.

**Năm thành phần thiết yếu** để thực thi chuyển đổi số (Chamorro-Premuzic, 2021, HBR — "mua công nghệ không tự tạo ra chuyển đổi"):
1. **People** — chuyển đổi số bắt đầu từ con người;
2. **Data** — "datafying" hành vi con người thành tín hiệu chuẩn hóa = digitisation;
3. **Insights** — analytics biến dữ liệu thành ý nghĩa;
4. **Action** — quyết định vẫn do con người; cần kỹ năng, quy trình và [[Change Management]];
5. **Results** — đánh giá kết quả, lặp lại để insight ngày càng dự báo tốt hơn.

**Ba chủ đề cơ hội chính** (Westerman et al., 2011): customer experience và [[Service Design]]; business & organisational processes; business models. Ví dụ business model: Netflix từ cho thuê DVD sang streaming; Domino's với mobile app và online ordering; GE với Industrial IoT; Volvo tăng năng lực sản xuất 90% nhờ automation, robotics và AI.

### Ví dụ thực tế
[[Case 10.2 NHS]] — EHR, telemedicine, patient portals, mHealth; [[Mini 10.3 Hertz]] — app di động, kiosk tự phục vụ, data analytics để cạnh tranh với Uber/Lyft.

### Liên kết
- [[Digital Transformation]] · [[Customer Experience]] · [[Service Design]] · [[Business Model]] · [[Data Analytics]]

---

## The Framework of Digital Transformation (Khung quy trình chuyển đổi số)

### Định nghĩa (Definition)
Các dự án chuyển đổi số thành công chia sẻ những chủ đề quy trình chung (Nylén & Holmström, 2015) mang tính **lặp (iterative)**: review → strategy → resourcing & planning → deployment → living with & evaluating.

### Giải thích chi tiết
**The process of review** — bốn câu hỏi xem xét đồng thời:
- **What the digital opportunity is**: environmental scanning thường xuyên, nhìn cả công nghệ, văn hóa, quy trình, kỹ năng.
- **How sure the organisation is**: opportunity analysis (tăng trưởng khách hàng? doanh thu kỳ vọng? giá trị cho khách hàng?) + success assurance (công nghệ ổn định? scale được? an toàn?).
- **Digital skills của leadership**: digital leaders thường chuyên sâu hẹp, broad-based leaders hiểu tổ chức nhưng thiếu trải nghiệm số — cần cả hai.
- **[[Digital Maturity]]**: đo bằng digital maturity index để benchmark theo ngành; mô hình BCG Digital Organisation Maturity: từ ad hoc → tập trung hóa (bổ nhiệm Chief Digital Officer) → hybrid với centres of excellence (CoE) → nhúng năng lực số toàn tổ chức. Checklist thiết kế tổ chức số (Moller et al., 2018): customer-centric, agile, experimental, lean/simple/standard, operational excellence, empowered & accountable, cross-functional.

**The process of strategy**: future-focused (nhắm cơ hội, không chỉ sửa vấn đề), time-frames ngắn (tuần/tháng thay vì kế hoạch 5 năm), objective alignment với chiến lược kinh doanh tổng thể.

**The process of resourcing and planning**: thiết kế transformation (chọn công nghệ: cloud, big data, AI, IoT; thiết kế lại quy trình qua [[Value Stream Mapping]]) + programme for change (assess current state → vision & strategy → prioritise → roadmap → secure buy-in → implement & measure → continuously improve).

**The process of deployment**: dự án nhỏ, nhanh nên dùng [[Agile]] (12 nguyên tắc Agile Manifesto, Beck 2001) thay vì quản lý dự án truyền thống; hackathons cũng được dùng cho dự án chuyển đổi nhỏ.

**The process of living with & evaluating**: chỉ 1/8 chuyển đổi số hoàn toàn thành công, hơn một nửa thất bại hoàn toàn (Gale, 2016). Đánh giá lặp lại các câu hỏi ban đầu (tăng trưởng, doanh thu, giá trị, khả năng scale) và revisit digital maturity index.

### Ví dụ thực tế
[[Case 10.3 Pfizer]] — Digital Centers of Excellence, in-transit visibility cho 20.000 chuyến hàng không + 2.000 đường biển + 35.000 đường bộ; T-Rex Solutions (SME): cloud AWS + Agile + RPA giúp giảm 40% chi phí hạ tầng, tăng 30% doanh thu — chuyển đổi số không chỉ dành cho tổ chức lớn; UK Government Digital Service với Digital Marketplace và Service Standard 18 tiêu chí.

### Liên kết
- [[Digital Maturity]] · [[Agile]] · [[Value Stream Mapping]] · [[Change Management]] · [[Digital Skills]]

---

## Key Issues in Digital Transformation (Các vấn đề then chốt)

### Định nghĩa (Definition)
Solis (2016) đưa ra **six stages of digital transformation** — khung đánh giá tiến độ trưởng thành chuyển đổi số của tổ chức.

### Giải thích chi tiết
Sáu giai đoạn (kèm ví dụ trong sách):
1. **Business as usual** — nhà bán lẻ địa phương chỉ dùng marketing truyền thống, chưa có e-commerce;
2. **Present and active** — nhà sản xuất có IoT sensors nhưng dữ liệu chưa tích hợp vào chiến lược;
3. **Formalised** — nhà cung cấp y tế có chiến lược chính thức, đầu tư EHR và telemedicine;
4. **Strategic** — công ty tài chính có đội chuyển đổi số chuyên trách, mobile banking, chatbots;
5. **Converged** — chuỗi bán lẻ tích hợp số toàn bộ từ SCM đến POS, mọi nhân viên được đào tạo;
6. **Innovative and adaptive** — công ty công nghệ liên tục thử nghiệm AI, blockchain.

**[[Value Stream Mapping]]**: kỹ thuật lean manufacturing để trực quan hóa các bước quy trình, xác định nơi tạo giá trị và nơi lãng phí; trong chuyển đổi số dùng để phát hiện điểm kém hiệu quả, tối ưu quy trình và giám sát tiến bộ. Sáu value streams thúc đẩy chuyển đổi số (Rossen): continuous build & test, continuous deployment, predictive service management, continuous feedback, continuous exploration, service onboarding & consumption. Ví dụ BankX (ngân hàng giả định): value stream mapping phát hiện nhập liệu thủ công trùng lặp → tự động hóa bằng machine learning, tích hợp hệ thống.

**Digital transformation excellence** — 6 yếu tố thành công (Westerman et al., 2014; Newman, 2019): leadership & vision, customer focus, agility & flexibility, data & analytics, talent & culture, technology infrastructure. Netflix minh họa: cá nhân hóa bằng ML giúp 57% thuê bao "extremely satisfied" (so 48% Hulu, 40% Amazon Prime Video), hơn 200 triệu thuê bao toàn cầu (2021).

**Bốn thách thức chính**: resistance to change (NHS gặp kháng cự từ nhân viên y tế); [[Legacy Systems]] và hạ tầng (Lufthansa 2011); data management & governance (Equifax 2017 rò rỉ dữ liệu vì không vá lỗ hổng); skills & talent gap (Volkswagen 2015 khó tuyển nhân tài số). Thất bại điển hình: Target Canada — mở hơn 100 cửa hàng 2011, đóng toàn bộ sau 2 năm do đánh giá thấp độ phức tạp thị trường, quản lý chuỗi cung ứng kém — cho thấy tầm quan trọng của phân tích môi trường vĩ mô (Chương 4).

### Ví dụ thực tế
[[Case 10.4 Walmart]] — Global eCommerce division (2011), Site-to-Store hơn 10 triệu đơn, smart shelving; [[Mini 10.5 Adidas]] — change management 4 trụ cột, online revenue tăng 50% năm 2019.

### Liên kết
- [[Value Stream Mapping]] · [[Digital Maturity]] · [[Legacy Systems]] · [[Data Governance]]

---

## Growth Hacking and Strategic Agility (Growth hacking và linh hoạt chiến lược)

### Định nghĩa (Definition)
[[Growth Hacking]] là kỹ thuật marketing nhằm tăng trưởng doanh nghiệp nhanh và hiệu quả bằng chiến thuật phi truyền thống, sáng tạo, tận dụng công nghệ và dữ liệu. [[Strategic Agility]] là văn hóa sẵn sàng thử nghiệm, chấp nhận rủi ro và pivot nhanh theo phản hồi và dữ liệu.

### Giải thích chi tiết
- Growth hacking là **mindset** hơn là danh sách kỹ thuật: đặt mục tiêu tăng trưởng không cần ngân sách marketing, dùng thời gian + sáng tạo (PR, social media). Không chỉ cho start-up công nghệ — Regus, Penguin Books cũng áp dụng.
- **Agile marketing / [[Scrum]]**: thay vì kế hoạch marketing lớn, chạy "Test, Learn and Commit" loops; 69% lãnh đạo B2B marketing nói điều kiện thay đổi quá nhanh để giữ kế hoạch hiện hành (Forrester, 2013); best practice chu kỳ lập kế hoạch không quá 90 ngày.
- **Growth hacking process** (Hemphill, 2020): **Stage 1 — [[Product-Market Fit]]**: chỉ growth hack sau khi đạt PMF; dùng lean start-up với minimum viable product; sản phẩm cần "hard push" để bán tức là chưa đủ tốt. **Stage 2 — Growth hacking**: câu hỏi duy nhất "làm gì để tăng trưởng cao, nhanh, rẻ?"; chạy tight tests, ghi lại mọi thí nghiệm, data-informed thay vì gut feel.
- **20 traction channels** (Weinberg & Mares 19 + 1) để thử nghiệm ra khỏi vùng an toàn; ưu tiên hóa bằng **AAARR pirate metrics** của Dave McClure: Acquisition → Activation → Retention → Revenue → Referral.
- [[Conversion Rate Optimisation]] khác "analyse and test" ở chỗ thiên về chiến lược và mindset; là hỗn hợp copywriting, [[SEO]], [[PPC]], social media, UX và tâm lý học; xếp kênh theo bucket [[Owned Earned Paid Media]].
- **Data analysis**: kết hợp định lượng (chuyện gì xảy ra) và định tính (tại sao); công cụ: Google Analytics, Mixpanel, Kissmetrics, Optimizely, Hotjar/SessionCam...

### Ví dụ thực tế
Airbnb growth hack kinh điển: reverse-engineer form của Craigslist (không có public API) để cross-post listing, tận dụng hàng triệu người dùng — "piggybacking" giống PayPal với eBay, Zynga với Facebook; hack tốt có vòng đời ngắn trước khi bị sao chép.

### Liên kết
- [[Growth Hacking]] · [[Product-Market Fit]] · [[Agile]] · [[Scrum]] · [[Conversion Rate Optimisation]] · [[AB Testing|A/B Testing]] · [[Web Analytics]]

---

## Adopting Digital Technologies (Áp dụng công nghệ số: dữ liệu và tự động hóa)

### Định nghĩa (Definition)
[[Data Analytics]] là quá trình rút trích insight có ý nghĩa từ dữ liệu để hỗ trợ ra quyết định — thành phần cốt lõi của chuyển đổi số.

### Giải thích chi tiết
- **Bốn loại analytics** (Davenport & Harris, 2017): descriptive (mô tả quá khứ) → predictive (dự báo) → prescriptive (khuyến nghị hành động) → autonomous (hệ thống tự học, tự cải thiện); độ tinh vi tăng dần theo analytics maturity model.
- **[[Big Data]]**: dữ liệu quá lớn/phức tạp cho công cụ truyền thống; chia structured / unstructured / semi-structured. Ba nhóm thách thức theo vòng đời dữ liệu (Sivarajah et al., 2016): data challenges (volume, variety, velocity, veracity...), process challenges (thu thập, tích hợp, chuyển đổi, chọn mô hình), management challenges (privacy, security, governance, đạo đức).
- Dữ liệu chuyển đổi doanh nghiệp qua: cá nhân hóa trải nghiệm khách hàng (tăng loyalty và doanh thu), tối ưu vận hành và giảm chi phí (phân tích chuỗi cung ứng).
- **Automated processes**: từ nhập liệu đơn giản đến workflow đa hệ thống; **RPA** cho tác vụ lặp lại, machine learning cho quyết định; giải phóng nhân viên cho việc chiến lược.
- **Integrated digital technologies**: kết hợp [[CRM]] + dữ liệu nhân khẩu/hành vi cho customer insight; predictive analytics cho dự báo nhu cầu; dữ liệu khảo sát + social media + review cho phát triển sản phẩm.

### Ví dụ thực tế
Pfizer dùng ML phân tích dữ liệu thử nghiệm lâm sàng để rút ngắn thời gian phát triển thuốc; Walmart dùng AI/ML tối ưu tồn kho.

### Liên kết
- [[Big Data]] · [[Data Analytics]] · [[Artificial Intelligence|AI and Machine Learning]] · [[CRM]] · RPA

---

## Change Management for Digital Transformation (Quản trị thay đổi)

### Định nghĩa (Definition)
[[Change Management]] là năng lực dẫn dắt con người, văn hóa và quy trình qua thay đổi — yếu tố phân biệt digital transformation với technology adoption. 50% sáng kiến thay đổi thất bại, chỉ 34% thành công rõ ràng (Gartner, 2018).

### Giải thích chi tiết
- Cân nhắc chính: leadership, culture, communication, training, data management.
- **Kotter 8 bước** áp dụng cho chuyển đổi số: (1) tạo cảm giác cấp bách, (2) lập guiding coalition, (3) xây vision & strategy, (4) truyền thông vision, (5) trao quyền hành động, (6) tạo short-term wins, (7) củng cố thành quả và tạo thêm thay đổi, (8) neo cách làm mới vào văn hóa.
- **Phổ thay đổi** (Harvard Business School Online, 2020): **Adaptive change** — điều chỉnh nhỏ, tăng dần (thêm phương thức thanh toán, nâng cấp phần mềm) đòi hỏi nhà quản lý methodical/analytical; **Transformational change** — thay đổi cấu trúc căn bản (brick-and-mortar → omnichannel, redesign website từ đầu) đòi hỏi persuader/visionary; đa số thay đổi nằm **ở giữa** phổ.
- **Open-source change management** (Gartner; Chiu & Salerno, 2019): hơn 80% tổ chức quản lý thay đổi top-down nhưng cách này không còn hiệu quả; áp dụng nguyên tắc open source tăng xác suất thành công từ 34% lên 58% qua ba cách: co-create change strategy (74% lãnh đạo nói có involve nhân viên nhưng chỉ 42% nhân viên cảm thấy được tham gia thật), shift implementation planning cho nhân viên (+12% xác suất thành công; ví dụ công ty phần mềm 20.000 người realign ưu tiên trong 6 tuần), focus communication on "talking" not "telling" (top-down làm tăng giận dữ, lo âu, kháng cự).

### Ví dụ thực tế
[[Mini 10.5 Adidas]]: chương trình change management 4 khu vực (leadership, culture, communication, training) song hành chuyển đổi số → online revenue +50% (2019), tổng doanh thu +13%.

### Liên kết
- [[Change Management]] · Kotter 8-Step Model · [[Digital Transformation]] · [[Digital Skills]]

---

## Monitoring and Governance (Giám sát và quản trị chuyển đổi số)

### Định nghĩa (Definition)
[[Data Governance]] là khung quản lý tài sản dữ liệu bảo đảm chúng được dùng hiệu quả cho kết quả kinh doanh. Gartner (2022): đến 2025, 80% tổ chức muốn scale digital business sẽ **thất bại** vì không có cách tiếp cận hiện đại với data governance.

### Giải thích chi tiết
- Các bước data governance: xác định mục tiêu → thiết lập chính sách (chất lượng, bảo mật, privacy, tuân thủ) → khung governance (vai trò, quy trình, công cụ) → data catalogue → data stewardship (gán chủ sở hữu dữ liệu) → quy trình quản lý (data quality, lineage, usage tracking).
- **COBIT** (ISACA): khung IT governance với 5 domain (Governance, Management, Risk, Control, Monitoring) và 37 quy trình IT trong 4 nhóm (Plan & organise, Acquire & implement, Deliver & support, Monitor & evaluate).
- **Adaptive data governance** (Gartner, 2022): phối hợp 4 phong cách theo bối cảnh — Control (rules, [[GDPR]], MDM), Outcomes (cân bằng rủi ro/lợi nhuận), Agility (trao quyền quyết định phân tán), Autonomous (quyết định real-time bởi người và "things").
- **Digitising core [[Legacy Systems]]**: hiểu yêu cầu kinh doanh → đánh giá IT landscape → định chiến lược → ưu tiên chuyển đổi tăng dần (phased) → tập trung data management → dùng [[Agile]]; Gartner (2019) đề xuất quy trình đánh giá 3 bước cho application modernisation.
- **Project management**: scope rõ, kế hoạch toàn diện, engage stakeholders, giám sát hiệu suất, đánh giá kết quả.
- **Evaluating success**: nhìn toàn diện qua customer experience, employee engagement, hiệu quả vận hành và hiệu quả tài chính để đo ROI.

### Ví dụ thực tế
Equifax (2017): vi phạm dữ liệu hàng triệu khách hàng do không vá lỗ hổng — bài học về data governance; [[Case 10.4 Walmart]] đo thành công qua đơn hàng Site-to-Store, giảm tồn kho và lãng phí.

### Liên kết
- [[Data Governance]] · COBIT · [[Legacy Systems]] · [[GDPR]] · [[Big Data]]

---

## Liên kết chương (Chapter Links)

- Chương trước: [[CH09 - Digital Experience and Service Design]] (customer experience — khu vực chuyển đổi số then chốt)
- Nền tảng chiến lược: [[CH05 - Digital Business Strategy]] · môi trường vĩ mô: [[CH04 - Key Issues in the Digital Environment]]
- Buy-side: [[CH06 - Digital Supply Chain Management]]
- Case studies: [[Case 10.1 Counterfeit Drugs Africa]] · [[Case 10.2 NHS]] · [[Case 10.3 Pfizer]] · [[Case 10.4 Walmart]] · [[Mini 10.1 Siemens]] · [[Mini 10.2 Carrefour]] · [[Mini 10.3 Hertz]] · [[Mini 10.5 Adidas]]
