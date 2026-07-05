---
tags: [chapter-9, part3, digital-experience, UX, usability, CRO, security, big-data, CRM]
aliases: [Thiết kế trải nghiệm và dịch vụ số, Digital Experience and Service Design, IDT Chapter 9]
---
# Chapter 9 - Digital Experience and Service Design

## Tổng quan (Overview)

Chương 9 mở đầu Part 3 (Implementation), tập trung vào các yếu tố thành công khi xây dựng trải nghiệm số hướng khách hàng (customer-facing digital experience) trên website và mobile app. Điểm xuất phát là [[Customer Journey]] — hay phễu chuyển đổi e-commerce (e-commerce conversion funnel): từ lúc khách truy cập trang chủ, tìm kiếm/duyệt sản phẩm, thêm vào giỏ đến khi thanh toán, mỗi bước đều có tỷ lệ rơi rụng (drop-off) mà nhà quản lý phải phân tích và tối ưu.

Chương đi qua chuỗi chủ đề thực hành: các khung đánh giá chất lượng dịch vụ online (WEBQUAL, E-SERVQUAL), [[Conversion Rate Optimisation]] với [[AB Testing|A/B Testing]] và [[Personalisation]], khung [[Customer Experience]] và [[Net Promoter Score]], [[Usability]] và [[Accessibility]], phân tích [[Personas]]/scenario/use-case, các kỹ thuật thiết kế mobile (responsive, adaptive, AMP, PWA, native app), [[Information Architecture]], hiệu năng website, hệ thống thanh toán, thiết kế bảo mật e-commerce, ứng dụng [[Big Data]] – [[Artificial Intelligence]] – [[Machine Learning]], và cuối cùng là [[CRM]] cho e-commerce với [[Permission Marketing]].

Thông điệp xuyên suốt: thiết kế trải nghiệm không phải khoản đầu tư một lần khi làm site mới, mà là quá trình cải tiến liên tục dựa trên dữ liệu ([[Web Analytics]]), thử nghiệm có cấu trúc và lắng nghe khách hàng.

---

## Frameworks Defining Effective Digital Experiences (Khung đánh giá trải nghiệm số hiệu quả)

### Định nghĩa (Definition)
Các framework chất lượng dịch vụ online giúp doanh nghiệp đánh giá mức chênh lệch giữa kỳ vọng của khách hàng và những gì đang được cung cấp — gọi là **online service–quality gap**.

### Giải thích chi tiết
Hai framework kinh điển:
- **WEBQUAL** (Loiacono et al.) — 14 chiều: information quality, functional fit to task, tailored communications, trust, response time, ease of understanding, intuitive operations, visual appeal, innovativeness, emotional appeal, consistent image, online completeness, relative advantage, customer service. Bị phê bình là thiên về thiết kế chức năng hơn dịch vụ.
- **E-SERVQUAL** (Zeithaml et al.) — 7 chiều: 4 chiều lõi (efficiency, fulfilment, reliability, privacy) + 3 chiều phục hồi (responsiveness, compensation, contact).

Năm yếu tố quyết định chất lượng dịch vụ theo [[SERVQUAL]] áp dụng online:
- **Tangibles**: ease of use + visual appeal của thiết kế.
- **Reliability**: mức sẵn sàng (availability) của website; khảo sát Superoffice (2017) trên 500 công ty: 41% không trả lời yêu cầu CSKH, 90% không xác nhận đã nhận email, 99% không follow-up, chỉ 11% trả lời đủ cả hai câu hỏi ngay lần đầu; thời gian phản hồi trung bình 15 giờ.
- **Responsiveness**: tốc độ phản hồi và tốc độ tải trang.
- **Assurance**: chất lượng phản hồi + bảo mật thông tin (chứng nhận ISIS, TrustArc, McAfee Scan Alert).
- **Empathy**: cá nhân hoá qua email/web.

Sở thích kênh đa dạng theo thế hệ (CMO Council 2019, khảo sát 2.000+ người tiêu dùng): 59% đồng ý "omnichannel" quan trọng; 3 thuộc tính khiến một kênh không thể thiếu: tiện lợi (50%), tin cậy (45%), tốc độ (41%); top kênh kỳ vọng: email 86%, điện thoại 65%, website 53%, text 52%, gặp trực tiếp 48%.

Ba bước quản trị theo SERVQUAL: (1) hiểu kỳ vọng khách hàng, (2) đặt và truyền thông lời hứa dịch vụ (nên under-promise, over-deliver), (3) thực hiện lời hứa qua on-site service, nhân viên và fulfilment.

### Ví dụ thực tế
Amazon đặt kỳ vọng giao hàng miễn phí trong 3 ngày rồi dùng nhiều phương thức giao để vượt kỳ vọng — trường hợp xấu nhất vẫn đúng hạn đã hứa.

### Liên kết
- [[Customer Experience]], [[SERVQUAL]], [[Omnichannel]], [[Personalisation]]

---

## Conversion Rate Optimisation, Merchandising and Personalisation (Tối ưu tỷ lệ chuyển đổi)

### Định nghĩa (Definition)
[[Conversion Rate Optimisation]] (CRO) là quá trình cải thiện hiệu quả thương mại của site giao dịch bằng cách tăng chuyển đổi tới các mục tiêu chính (bán hàng, báo giá, booking, lead), kết hợp nghiên cứu khách hàng/đối thủ với [[Web Analytics]], [[AB Testing|A/B Testing]] và [[Multivariate Testing]].

### Giải thích chi tiết
- Ngay cả các thương hiệu lớn có team merchandising chuyên trách, tỷ lệ chuyển đổi điển hình vẫn **dưới 1/10 khách truy cập** (dữ liệu Kibo) → dư địa tối ưu lớn ở từng bước: xem trang sản phẩm → add-to-cart → mua.
- KPI của test không chỉ là [[Conversion Rate]]: còn [[Bounce Rate]], average order value (AOV) và **revenue per visit (RPV)** — RPV được khuyến nghị cho retailer vì gộp cả conversion và AOV.
- Ưu tiên test bằng **PIE scoring** (Wider Funnel): Potential (cải thiện được bao nhiêu), Importance (traffic và conversion bị ảnh hưởng), Ease (dễ triển khai về kỹ thuật lẫn chính trị nội bộ).
- [[AB Testing|A/B Testing]]: so sánh 2 phiên bản trang/phần tử (heading, ảnh, nút) — "live split testing"; ABC test so 2 challenger với control; [[Multivariate Testing]] test đồng thời nhiều tổ hợp phần tử. Mỗi test cần hypothesis: "If I do X I think it will improve Y" và cần kiểm định ý nghĩa thống kê. Công cụ: Optimizely, VWO, Unbounce.
- **Forward/reverse path analysis** trong analytics giúp chọn trang cần cải thiện (landing page, checkout).
- [[Personalisation]]: dùng dữ liệu implicit (context: thiết bị, vị trí, nguồn referral; behaviours: sản phẩm đã xem, giỏ hàng bỏ dở) và explicit (form, survey). **Pyramid of personalisation** (Monetate/Kibo) 3 cấp: (1) optimisation bằng AB testing, (2) segmentation theo rule-based targeting, (3) 1:1 personalisation bằng [[Machine Learning]]/predictive analytics.
- **Online retail merchandising**: mở rộng navigation bằng synonym, faceted navigation, nêu bật best-seller (Top 10/20), bundling (BOGOF), ratings & reviews — case Bazaarvoice/CompUSA: reviews giúp conversion +60%, order value +50%, page views/visitor +82%.

### Ví dụ thực tế
Xero Shoes (Mini case 9.1): thêm product links lên trang chủ → RPV tăng 6,45%. Lyko (hair & beauty Thuỵ Điển, 30% khách dùng site search) dùng nền tảng personalisation Voyado Elevate để tự động hoá merchandising — xem [[Mini 9.5 Personalisation Providers]].

### Liên kết
- [[Conversion Rate Optimisation]], [[AB Testing|A/B Testing]], [[Multivariate Testing]], [[Personalisation]], [[Bounce Rate]], [[Mini 9.1 Xero Shoes]]

---

## Customer Experience Frameworks (Khung quản trị trải nghiệm khách hàng)

### Định nghĩa (Definition)
**Customer Experience Management (CXM)** là quản trị tích hợp các hệ thống tạo nên trải nghiệm (web content management, personalisation, marketing automation, commerce platform, customer service, on-site search, merchandising, analytics + testing) như một quá trình cải tiến liên tục.

### Giải thích chi tiết
- Nghiên cứu KPMG Nunwood: thương hiệu cải thiện [[Customer Journey]] tăng doanh thu **10–15%** và giảm cost-to-serve **15–20%**; tăng trưởng doanh thu + lợi nhuận của top 10 thương hiệu CX gấp **4 lần** bottom 10.
- **Six pillars of experience excellence** (từ 1,85 triệu đánh giá): Personalisation, Integrity, Expectations, Resolution, Time & Effort, Empathy. Chuyển đổi CX cần kế hoạch 3–5 năm tối thiểu.
- 10 lời khuyên triển khai CX (Econsultancy): định nghĩa CX tốt; bỏ tư duy theo kênh; lấy customer journey làm trung tâm; có người chịu trách nhiệm; xây thương hiệu để khác biệt; tự tạo framework (SWOT theo cấu phần CX); công nghệ là công cụ không phải giải pháp; đổi mới có chọn lọc; lãnh đạo (CEO) cam kết; bắt đầu ngay.
- Benchmark bằng chỉ số hài lòng: UK Customer Satisfaction Index, American Customer Satisfaction Index (ACSI 2023: retailer đạt 84% độ chính xác đơn hàng, 84% dễ pickup, 81% tốc độ chuẩn bị đơn).
- [[Net Promoter Score]] (Reichheld): "Would you recommend us?" thang 0–10; NPS = %Promoters (9–10) − %Detractors (0–6). Phân tích kinh tế của Dell: khách hàng trung bình đáng giá $210, detractor làm mất $57, promoter tạo ra $328. Cách tăng NPS online: nút forward-to-a-friend, chương trình email xin ý kiến, showcase trải nghiệm tích cực, quản lý detractor bằng reputation management. Phê bình: cùng một NPS có thể đến từ cơ cấu promoter/detractor rất khác nhau; ~3/4 khách nói sẽ giới thiệu nhưng chỉ ~1/3 làm thật và chỉ 13% referral tạo khách mới.

### Ví dụ thực tế
Uber và Airbnb đã "reset" kỳ vọng của khách hàng về gọi xe và lưu trú — buộc mọi tổ chức phải quản trị cách kỳ vọng hình thành và cách đáp ứng.

### Liên kết
- [[Customer Experience]], [[Net Promoter Score]], [[Customer Journey]], [[SWOT]]

---

## Usability for Desktop and Mobile (Tính khả dụng)

### Định nghĩa (Definition)
[[Usability]] (ISO Human-centred Design Processes for Interactive Systems): "mức độ một sản phẩm có thể được người dùng xác định sử dụng để đạt mục tiêu xác định với **effectiveness, efficiency và satisfaction** trong bối cảnh sử dụng xác định."

### Giải thích chi tiết
- **User-centred design (UX)** bắt đầu từ hiểu người dùng: họ là ai, mục đích truy cập, tần suất, kinh nghiệm, ngôn ngữ, loại thông tin cần, thiết bị/trình duyệt (Bevan).
- Bối cảnh sử dụng ngày càng đa dạng: smartphone, multi-screening, hành vi mua đa kênh, tích hợp social + email, live chat.
- Nielsen: "On the Web, usability is a necessary condition for survival... leaving is the first line of defense" — đề xuất dành **~10% ngân sách dự án thiết kế** cho usability.
- Hai hoạt động chính: **expert review** (đầu dự án redesign) và **usability testing**: (1) xác định người dùng đại diện + personas, (2) hỏi ý kiến về site hiện tại, (3) giao nhiệm vụ cụ thể (tìm sản phẩm, đặt hàng), (4) quan sát (focus group, heatmap, session recording như Hotjar), (5) tinh chỉnh và lặp lại.
- Đo lường: effectiveness (% hoàn thành nhiệm vụ), efficiency (thời gian/số click), satisfaction.
- **Top Tasks** (McGovern 2018): khảo sát ~400 người đủ xếp hạng 5 nhiệm vụ hàng đầu; top 4–5 tasks thường chiếm 25% phiếu bầu.
- **Exit intent survey** 4 câu: mục đích ghé thăm? hoàn thành chưa? mức hài lòng? nếu không thì vì sao? **Eyetracking** đánh giá hiệu quả thiết kế.
- 14 lý do doanh nghiệp thất bại với UX (Econsultancy): bỏ qua user research, coi nhẹ feedback, bỏ quên accessibility, ngại thay đổi, thiếu hợp tác liên phòng ban, thiếu đào tạo UX, mất cân bằng thẩm mỹ–chức năng, bỏ qua bối cảnh sử dụng, hạn chế ngân sách, văn hoá xem nhẹ UX, không dùng data để iterate, bỏ quên cảm xúc, lệch pha mục tiêu kinh doanh–nhu cầu người dùng, đánh giá thấp độ phức tạp của UX.

### Ví dụ thực tế
Built for Mars (2020) đo usability ngân hàng bằng số click mở tài khoản: ngắn nhất Revolut (24), Starling (38), Monzo (45); dài nhất First Direct (120), HSBC (99), Co-op (92) — xem [[Mini 9.3 Banking Usability]].

### Liên kết
- [[Usability]], [[Accessibility]], [[Personas]], [[Conversion Rate Optimisation]], [[Web Analytics]]

---

## Persona and Scenario Analysis (Phân tích persona và kịch bản)

### Định nghĩa (Definition)
[[Personas]] là bản mô tả "thumbnail" một kiểu khách truy cập điển hình; **customer scenario** (Seybold) là chuỗi nhiệm vụ persona đó cần làm để đạt kết quả mong muốn.

### Giải thích chi tiết
- Xây persona với thuộc tính: demographic (tuổi, giới, nghề; B2B thêm quy mô công ty, vai trò trong buying unit), psychographic (mục tiêu, động lực), webographics (kinh nghiệm web, thiết bị, tần suất).
- 3–4 persona thường đủ; chọn **primary persona** (quan trọng với business và "khó tính" về thiết kế); có secondary và complementary personas.
- Mỗi persona viết 3–4 scenario: tìm thông tin (→ đăng ký), mua lần đầu, mua lặp lại.
- **Use-case analysis** (Schneider & Winters) 4 bước: (1) identify actors (người/hệ thống tương tác), (2) identify use-cases (hành vi hệ thống cần hỗ trợ), (3) relate actors to use-cases, (4) develop use-case scenarios chi tiết với basic path / alternative paths, pre-condition và post-condition (ví dụ use-case "Register" của khách e-commerce).
- Card sorting ("knowledge elicitation") giúp xây menu đúng logic người dùng thay vì logic kỹ sư.

### Ví dụ thực tế
Miele Professional xây persona chủ care home/khách sạn SME từ data mining + phỏng vấn điện thoại ~10 câu, làm nền cho chiến dịch content marketing đạt ROI 321% — xem [[Mini 9.4 Miele]].

### Liên kết
- [[Personas]], [[Customer Journey]], [[Card Sorting]], [[Content Marketing]]

---

## Mobile Design Requirements and Techniques (Thiết kế cho mobile)

### Định nghĩa (Definition)
Smartphone là phương thức truy cập web chủ đạo (trừ B2B), nên thiết kế hiệu quả trên cả mobile lẫn desktop là yêu cầu bắt buộc; "mobile first" (Eric Schmidt, 2010) nhấn mạnh tối giản nhưng không phải phương pháp luận thống nhất.

### Giải thích chi tiết
Năm lựa chọn kỹ thuật:
1. **[[Responsive Design]] (RWD)**: một phiên bản site duy nhất, layout "chảy" theo độ phân giải nhờ CSS media queries — tiết kiệm nhất, phổ biến nhất với SME; nhược điểm: codebase CSS lớn, có thể chậm.
2. **Adaptive design**: kết hợp logic client/server để phục vụ code riêng cho từng thiết bị ưu tiên — nhanh hơn nhưng chi phí phát triển cao, hợp doanh nghiệp lớn.
3. **AMP (Accelerated Mobile Pages)**: tải cực nhanh do ít styling và phục vụ từ server Google; chủ yếu publisher dùng, mức chấp nhận hiện đã thấp.
4. **[[Progressive Web App]] (PWA)**: dùng modern API cho trải nghiệm như app (offline, cài lên màn hình chính) với một codebase duy nhất, không cần app store. Google: 53% phiên mobile bị bỏ nếu tải >3 giây. Kết quả thực tế: MakeMyTrip conversion ×3, session +160%; Alibaba.com conversion +76%, tương tác ×4; Lancôme session +53%, bounce −10%; Starbucks PWA song song native app.
5. **Native [[Mobile App]]**: cài từ App Store/Google Play, cá nhân hoá và gắn kết sâu nhất; hơn 90% thời gian mobile của người dùng nằm trong app nhưng chủ yếu là social/email/news. Fintech như Monzo, Revolut, Starling chọn mô hình app-only.

6 câu hỏi trước khi làm app: app có phải ưu tiên chiến lược? tự build hay tận dụng app sẵn có? free hay paid (freemium với in-app purchase)? nhắm category nào? quảng bá ra sao (App Store Optimisation, giới thiệu bạn bè, email)? cải tiến theo feedback thế nào?

### Ví dụ thực tế
Các ngân hàng challenger (Monzo, Starling) mở tài khoản hoàn toàn qua app trong 2 ngày làm việc, trong khi ngân hàng truyền thống chậm nhất mất 36 ngày.

### Liên kết
- [[Responsive Design]], [[Progressive Web App]], [[Mobile App]], [[Conversion Rate]]

---

## Information Architecture (Kiến trúc thông tin)

### Định nghĩa (Definition)
[[Information Architecture]] (Rosenfeld & Morville): sự kết hợp các hệ thống tổ chức, gán nhãn và điều hướng trong một hệ thống thông tin — thiết kế cấu trúc không gian thông tin để hỗ trợ hoàn thành nhiệm vụ và truy cập nội dung trực quan.

### Giải thích chi tiết
- Lợi ích: hỗ trợ [[Usability]] và "flow", cải thiện [[SEO]] (nhãn và nhóm nội dung có cấu trúc), tích hợp truyền thông offline (landing page), đo lường tốt hơn.
- **[[Card Sorting]]**: người dùng nhóm/xếp hạng thẻ (loại tài liệu, từ khoá, nhãn điều hướng) để tạo phân loại đúng mental model của họ.
- **Blueprints** (site map/site structure diagram): thể hiện quan hệ giữa các trang, nhóm nội dung và liên kết.
- **[[Wireframe]]** (schematic): phác thảo layout từng loại trang — vị trí navigation, header/footer, "slots" nội dung động; sau đó chuyển thành page template dùng **CSS** (lợi ích: tải nhanh hơn, phát triển hiệu quả, dễ bảo trì, tương thích đa trình duyệt, tăng accessibility).
- **Site organisation schemes**: exact (alphabet, thời gian, địa lý), ambiguous (theo chủ đề/nhiệm vụ/đối tượng — phổ biến nhất cho e-commerce, kèm ẩn dụ shopping basket), hybrid.
- **Navigation**: khái niệm **flow** (Hoffman & Novak; Csikszentmihalyi) — trạng thái đắm chìm khi tìm thông tin dễ dàng; yếu tố phá flow: tải chậm, form dài, link hỏng. Cân bằng narrow-and-deep vs broad-and-shallow; quy tắc **3 click**; chú ý deep linking (Nielsen) — người dùng không phải lúc nào cũng vào từ trang chủ. Ba câu hỏi điều hướng: Where am I? Where have I been? Where do I want to go?
- **Page design**: tỷ lệ content vs navigation, tránh frame, cho phép resize, nhất quán, hỗ trợ in ấn. **Content design**: viết ngắn gọn hơn brochure, chunking 5–6 dòng, dùng list và hyperlink; tránh giả định người đọc hiểu jargon nội bộ; 5 giai đoạn xử lý thông tin của Hofacker làm checklist.

### Ví dụ thực tế
Dell phân khúc audience ngay trang chủ (home user → corporate → government); menu system của một nhà sản xuất đồ chơi được thiết kế lại từ card sorting khác hẳn phương án kỹ sư phần mềm hình dung.

### Liên kết
- [[Information Architecture]], [[Card Sorting]], [[Wireframe]], [[SEO]], [[Usability]]

---

## Accessibility for E-commerce (Khả năng tiếp cận)

### Định nghĩa (Definition)
[[Accessibility]] là thiết kế cho phép mọi người dùng tương tác với website bất kể khuyết tật (đặc biệt khiếm thị dùng screen-reader), trình duyệt hay nền tảng truy cập.

### Giải thích chi tiết
- Bốn lý do đầu tư: (1) hàng triệu người khiếm thị (từ mù màu đến mù), (2) đa dạng trình duyệt/độ phân giải, (3) kỹ thuật accessibility đồng thời cải thiện [[SEO]] (text alternative, navigation rõ), (4) yêu cầu pháp lý — UK: Equality Act 2010 (Bắc Ireland: DDA 1995).
- Chuẩn tham chiếu: W3C **Web Accessibility Initiative (WAI)**.
- Quote đáng nhớ của người dùng screen-reader (RNIB): "For me being online is everything. It's my hi-fi, it's my source of income, it's my supermarket, it's my telephone. It's my way in."

### Ví dụ thực tế
RS Components áp dụng nguyên tắc accessibility + usability trong chuyển đổi customer-centric — xem [[Case 9.1 B2B UX]].

### Liên kết
- [[Accessibility]], [[Usability]], [[SEO]]

---

## Performance for E-commerce (Hiệu năng)

### Định nghĩa (Definition)
Tốc độ tải trang và mức sẵn sàng (availability) quyết định trực tiếp bounce rate, conversion và cả thứ hạng tìm kiếm (Google Core Web Vitals).

### Giải thích chi tiết
- Google: người dùng chấp nhận ~2 giây, website châu Âu trung bình ~8 giây; tải 1s→3s làm [[Bounce Rate]] tăng 32%, 1s→6s tăng 106%.
- Kỹ thuật cải thiện: lazy loading, minify/combine file để giảm HTTP request, định dạng ảnh thế hệ mới (WebP, JPEG 2000/XR), tối ưu phần tử trang (hạn chế carousel), CDN (Akamai, Cloudflare — kèm chống DDoS); HTTP/2 và HTTPS (Google ưu tiên xếp hạng site https).
- **Availability**: lý thuyết 100% nhưng thường thấp hơn; SciVisum khuyến nghị: định nghĩa throughput đỉnh cho từng customer journey (ví dụ 10 checkout/giây, 30 add-to-basket/giây), SLA chi tiết theo từng bước giao dịch, giám sát 24/7 (Pingdom, Uptrends cho SME).

### Ví dụ thực tế
RS Components cải thiện tốc độ faceted search nhanh hơn 70% (chọn 4 filter từ 10 giây còn 3,2 giây) → conversion từ search filtering tăng 40%.

### Liên kết
- [[Bounce Rate]], [[Web Analytics]], [[Conversion Rate]]

---

## Payment Systems for E-commerce (Hệ thống thanh toán)

### Định nghĩa (Definition)
Ngoài thẻ tín dụng/ghi nợ và PayPal, thanh toán e-commerce hiện đại gồm ví số/mobile wallet (Apple Pay, Google Pay; AliPay, WePay ở châu Á) và Buy Now Pay Later (Klarna, AfterPay, ClearPay).

### Giải thích chi tiết
- Merchant muốn cung cấp nhiều lựa chọn nhưng tránh chi phí tích hợp từng cổng riêng → dùng **payment processor** (Stripe, PayPal, Square) tích hợp qua API một lần, kèm 3D identity verification.
- **PCI DSS compliance** là yêu cầu của tổ chức phát hành thẻ (bắt buộc theo luật ở một số bang Mỹ); mức kiểm tra tuỳ số lượng giao dịch/năm; payment gateway và nền tảng e-commerce hỗ trợ tuân thủ.

### Ví dụ thực tế
Stripe (thành lập 2010 bởi anh em Collison) thu phí % mỗi giao dịch; Smart Insights chuyển từ PayPal sang Stripe nhờ form thanh toán tốt hơn, linh hoạt đổi sản phẩm/giá, báo cáo và công cụ PCI compliance.

### Liên kết
- Digital Wallet, [[FinTech]], [[Conversion Rate Optimisation]]

---

## Security Design for E-commerce (Thiết kế bảo mật)

### Định nghĩa (Definition)
Bảo mật thông tin (khách hàng và nội bộ) là mối quan tâm hàng đầu của quản lý digital business — vừa là yêu cầu pháp lý (luật bảo vệ dữ liệu, xem [[CH04 - Key Issues in the Digital Environment]]) vừa là yếu tố giữ niềm tin.

### Giải thích chi tiết
- UK Cyber Security Breaches Survey: 39% doanh nghiệp phát hiện tấn công/vi phạm trong 12 tháng (doanh nghiệp lớn: 72%). Google & McAfee ước tính ~2.000 cuộc tấn công mạng/ngày, thiệt hại ~£300 tỷ/năm toàn cầu.
- Sự cố lớn: **TalkTalk** (2015, DDoS + đánh cắp dữ liệu 156.959 khách, 15.656 số tài khoản; phạt £400.000 nhưng tổng thiệt hại ước £60 triệu + mất >100.000 khách hàng); **Uber** (2016, che giấu vụ hack 57 triệu người dùng, trả hacker $100.000 để xoá dữ liệu).
- **NCSC 9 bước**: bảo vệ mạng (firewall), đào tạo nhân viên, quản lý quyền truy cập, cập nhật phần mềm/patch, kiểm soát removable media, quy định mobile working (mã hoá, remote wipe), anti-malware, giám sát, quản lý sự cố + business continuity.
- Chuẩn **ISO/IEC 17799 (BS 7799)**: chu trình Plan–Do–Check–Act và 10 mục từ security policy, phân loại tài sản thông tin (information asset register), nhân sự, vật lý, vận hành, access control đến disaster recovery và compliance.
- 5 yêu cầu của giao dịch an toàn: **authentication, privacy/confidentiality, integrity, non-repudiability, availability**.
- Kỹ thuật: mã hoá **symmetric** (khoá bí mật chia sẻ — dùng cho EDI, không thực tế cho e-commerce đại chúng) vs **asymmetric/public-key** (cặp khoá công khai–riêng tư; PGP cho email). [[Digital Certificate]] và [[Digital Signature]] xác thực các bên; **PKI** với **certificate authorities (CAs)** (Symantec/Verisign, bưu điện, ngân hàng) phát hành chứng chỉ. **VPN** ("tunnelling" qua IPSec) cho mạng riêng trên hạ tầng công cộng. **[[SSL]]**: giao thức phổ biến nhất cho B2C (https:// + biểu tượng ổ khoá) — bảo mật đường truyền nhưng không tự xác thực khách hàng.

### Ví dụ thực tế
Câu hỏi lớn sau vụ TalkTalk: "Why wasn't the data encrypted?" — mã hoá dữ liệu lưu trữ là phòng tuyến cơ bản mà công ty đã bỏ qua.

### Liên kết
- [[Digital Certificate]], [[Digital Signature]], [[SSL]], [[GDPR]], [[Privacy]]

---

## Big Data, AI and Machine Learning for E-commerce (Dữ liệu lớn và AI)

### Định nghĩa (Definition)
[[Big Data]] là thuật ngữ chỉ các kỹ thuật phân tích và hệ thống khai thác khối lượng dữ liệu khổng lồ doanh nghiệp thu thập; đặc trưng bằng **4V của IBM**: Volume, Variety, Velocity, Veracity.

### Giải thích chi tiết
- IBM (2013): mỗi ngày tạo ra 2,5 quintillion bytes; 90% dữ liệu thế giới được tạo trong 2 năm gần nhất. Hadoop xử lý dữ liệu phi cấu trúc, khác data warehouse truyền thống có cấu trúc chặt.
- Hai lợi ích marketing: tìm insight (trend, pattern) từ tập dữ liệu lớn liên kết; tăng độ liên quan của truyền thông (timing, copy, offer).
- **15 ứng dụng [[Artificial Intelligence]] trong marketing** (theo vòng đời khách hàng RACE): AI-generated content/NLG (AP tạo ~4.000 bài earnings/quý — gấp 12 lần thủ công; Vivint tăng 5× sales nhờ localised pages; Phrasee tối ưu subject line email), smart content curation (Netflix recommendations), voice search & conversational UI (Alexa), programmatic media bidding, propensity modelling, [[Predictive Analytics]], lead scoring, ad targeting, dynamic pricing, web & app personalisation, [[Chatbot]] (Pizza Express đặt bàn qua Facebook Messenger; bùng nổ sau ChatGPT 2022–2023), re-targeting, predictive customer service, marketing automation, 1:1 dynamic content email.
- Cảnh báo: propensity model chỉ tốt bằng dữ liệu đầu vào; case Target (Mỹ) dự đoán thai kỳ từ hành vi mua — gửi thư "cribs and bibs" cho thiếu niên trước khi cô báo với gia đình → rủi ro đạo đức/privacy.
- **[[IoT]] và M2M**: sản phẩm kết nối gồm 3 lớp (physical + smart + connectivity components — Porter & Heppelmann); ứng dụng marketing: products as media, products as a service, products as connected ecosystems. EVRYTHNG × Avery Dennison đưa ≥10 tỷ sản phẩm may mặc "born digital" trong 36 tháng; adidas bán ~1,3 triệu đôi giày/ngày muốn theo dõi vòng đời từng sản phẩm.
- [[Virtual Reality]], [[Augmented Reality]] và [[Metaverse]]: đã trình bày ở [[CH04 - Key Issues in the Digital Environment]].

### Ví dụ thực tế
Diageo Brasil kết nối 100.000 chai whisky với Internet cho thông điệp video cá nhân hoá dịp Father's Day: sales tăng 72%, chi phí chiến dịch hoàn vốn 5 lần — xem [[Mini 9.6 EVRYTHNG Diageo]].

### Liên kết
- [[Big Data]], [[Artificial Intelligence]], [[Machine Learning]], [[Predictive Analytics]], [[Chatbot]], [[IoT]], [[Personalisation]]

---

## Customer Relationship Management for E-commerce (CRM cho e-commerce)

### Định nghĩa (Definition)
[[CRM]] liên kết thông tin khách hàng từ nhiều nguồn (email, website, cửa hàng, call center, mobile, quảng cáo) giữa hệ thống vận hành và phân tích để hiểu và đáp ứng nhu cầu khách hàng, tăng doanh thu. Phiên bản số hoá từng gọi là [[eCRM]], nay đơn giản là CRM.

### Giải thích chi tiết
- Kinh tế học giữ chân khách (Reichheld & Schefter): chi phí thu hút khách online cao hơn truyền thống 20–30%; giữ thêm 5% khách hàng có thể tăng lợi nhuận 25–95%. (Reinartz & Kumar phản biện: khách trung thành không hẳn rẻ hơn để phục vụ.)
- 6 kỹ thuật tạo loyalty cho online retailer: nurturing brand preference, re-sell, [[Cross-selling]], [[Upselling]], reactivation, referrals.
- 5 ứng dụng marketing của hệ CRM: salesforce automation (SFA), customer service management, quản lý sales process, campaign management, analysis (data warehouse + data mining).
- Lợi ích: targeting chính xác hơn (danh sách tự chọn lọc/pre-qualified), mass customisation thông điệp, tăng chiều sâu quan hệ, learning relationship (như Amazon), chi phí thấp hơn direct mail.
- **Customer engagement**: "repeated interactions that strengthen the emotional, psychological or physical investment a customer has in a brand" — thách thức trung tâm khi attention khan hiếm.
- **[[Permission Marketing]]** (Seth Godin): đối lập interruption marketing; con người nhận >3.000 thông điệp marketing/ngày; nguyên tắc "dating the customer": incentive để volunteer → dạy dần về sản phẩm → củng cố incentive → mở rộng permission → chuyển hành vi thành lợi nhuận. Cơ chế **opt-in** (chủ động đồng ý) được luật bảo vệ dữ liệu nhiều nước bắt buộc thay cho opt-out.
- Quy trình xây quan hệ 4 bước: attract (inbound + paid media) → prompt/incentivise action (lead offer, sales offer, pop-up — pop-up của Smart Insights tăng lead conversion 40%) → capture thông tin qua form tối ưu (KISS, WIFM, privacy "we will not share") → maintain dialogue (email, personalisation).
- **Live chat**: giảm chi phí contact center, một nhân viên xử lý nhiều chat đồng thời.

### Ví dụ thực tế
Warby Parker xây dựng quan hệ khách hàng qua chuỗi email automation bám sát từng bước Home Try-On, video trả lời cá nhân hoá trên Twitter (retweet gấp 65 lần tweet thường) và CRM tích hợp online–offline — xem [[Case 9.2 Warby Parker]]. Tony's Chocolonely dùng nền tảng số để biến khách thành người vận động chống nô lệ trẻ em trong ngành cacao — xem [[Mini 9.7 Tony's Chocolonely]].

### Liên kết
- [[CRM]], [[eCRM]], [[Permission Marketing]], [[Email Marketing]], [[Customer Lifetime Value]], [[Cross-selling]], [[Upselling]], [[Social Media Marketing]]

---

## Case studies của chương
- [[Case 9.1 B2B UX]] — RS Components: chuyển đổi UX customer-centric trong B2B
- [[Case 9.2 Warby Parker]] — disrupt ngành kính mắt bằng D2C + CX
- [[Mini 9.1 Xero Shoes]] — CRO tăng revenue per visit
- [[Mini 9.3 Banking Usability]] — đo usability ngân hàng bằng số click
- [[Mini 9.4 Miele]] — persona-driven content marketing B2B
- [[Mini 9.5 Personalisation Providers]] — Lyko × Voyado Elevate
- [[Mini 9.6 EVRYTHNG Diageo]] — IoT connected products
- [[Mini 9.7 Tony's Chocolonely]] — CRM/advocacy vì mục tiêu đạo đức

## Liên kết chương
- Trước: [[CH08 - Digital Communications]] (6 kênh truyền thông số đưa khách đến trải nghiệm)
- Sau: [[CH10 - Managing Digital Transformation]] (growth hacking + CRO ở cấp tổ chức)
- Nền tảng pháp lý bảo mật/privacy: [[CH04 - Key Issues in the Digital Environment]]
