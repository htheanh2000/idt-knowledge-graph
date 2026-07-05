---
tags: [chapter-3, part1, e-commerce, B2C, B2B, C2C, headless, payment, marketplace, security, UX]
aliases: [Quản trị Thương mại điện tử, E-commerce Management, IDT Chapter 3]
---
# Chapter 3 - E-commerce Management

## Tổng quan (Overview)

Chương 3 đi sâu vào [[E-commerce]] như một tập con của [[Digital Business]]: mọi tổ chức e-commerce đều là digital business, nhưng không phải digital business nào cũng có yếu tố e-commerce. Trọng tâm của e-commerce là **transaction** (giao dịch) — các giao dịch thương mại được **digitally enabled** giữa doanh nghiệp với người tiêu dùng ([[B2C]]), giữa các doanh nghiệp ([[B2B]]) và giữa người tiêu dùng với nhau ([[C2C]]).

Chương trình bày chiến lược e-commerce (value proposition, 5 [[Revenue Model]], 6 operating model), quá trình phát triển nền tảng e-commerce (bao gồm xu hướng [[Headless E-commerce]] và hệ thống thanh toán như [[Buy Now Pay Later]]), đặc thù của B2C retail, B2B, content e-commerce, [[Marketplace]] và đấu giá trực tuyến, các vấn đề bảo mật, và cuối cùng là bộ best practice thiết kế platform để tăng conversion (điều hướng, [[Call To Action]], [[Trust Signals]], [[SEO]] cho product page).

Học xong chương này, bạn có thể đề xuất một e-commerce proposition hoàn chỉnh, chọn mô hình vận hành và nền tảng phù hợp, đồng thời biện giải các quyết định triển khai.

---

## An Introduction to E-commerce (Giới thiệu về E-commerce)

### Định nghĩa (Definition)
[[E-commerce]] là việc sử dụng Digital để **thực hiện giao dịch thương mại** (transact). Kalakota & Whinston (1997) xác định 4 góc nhìn kinh điển vẫn còn giá trị: (1) electronic communications — truyền thông tin/sản phẩm/thanh toán bằng phương tiện điện tử; (2) e-commerce business process — tự động hóa giao dịch và workflow; (3) electronic service — giảm chi phí, tăng tốc độ và chất lượng dịch vụ; (4) online nature — mua bán trực tuyến theo nghĩa đen.

### Giải thích chi tiết
Bốn nguyên lý chính của e-commerce hiện đại:
- **Time and space agnosticism**: truy cập được 24/7/365 từ bất kỳ đâu, không cần hai bên hiện diện đồng thời.
- **Widely available standard approaches**: dùng phần cứng/phần mềm chuẩn, không đòi hỏi add-on độc quyền.
- **Availability and complexity of information**: thông tin sản phẩm dồi dào giúp so sánh dễ hơn; ngược lại doanh nghiệp thu insight hành vi khách hàng ở quy mô lớn ([[Big Data]]).
- **Interactivity and individualisation**: cá nhân hóa nội dung và sản phẩm tới từng khách hàng (customise giày, bundle riêng, cấu hình xe) — nền tảng của one-to-one marketing.

Ba loại e-commerce chính:
- **[[B2C]]**: kết nối với người tiêu dùng cá nhân — retail, travel ([[Online Travel Agents]]), finance, bất động sản, dịch vụ.
- **[[B2B]]**: giao dịch giữa các doanh nghiệp — quy mô doanh thu **lớn hơn B2C một bậc độ lớn**.
- **[[C2C]]**: người tiêu dùng giao dịch với nhau — eBay, TaoBao, Vinted, Facebook Marketplace; Uber và Airbnb tự xếp mình là marketspace C2C.

Các hình thái bổ sung: [[Mobile Commerce]] (native app ngày càng thay web), Conversational Commerce qua Messenger/WhatsApp với chatbot, [[Social Commerce]] (nút Buy Now, shopping tab), [[Livestreaming Commerce]] (TikTok, phổ biến nhất ở Trung Quốc) và Local E-commerce (voucher, giao đồ ăn, gọi xe).

Tiến hóa: từ giao dịch qua modem và [[EDI]], Minitel (Pháp, 1981) → thương mại hóa Internet giữa thập niên 1990 (Amazon 1994, Zappos 1999) → dịch vụ tài chính online đầu 2000s → iPhone 2007 mở kỷ nguyên mobile.

**Emerging themes 2020s**: COVID-19 tạo cú nhảy đột biến — tại Mỹ, e-commerce từ 11,1% (2019) lên 14,2% tổng retail sales cuối 2020; tại UK gần gấp đôi lên ~25%. Nhưng sau lockdown nhu cầu giảm mạnh về lại đường xu hướng cũ; Shopify phải cắt 10% nhân sự năm 2022 vì đặt cược sai rằng mức tăng là vĩnh viễn. Xu hướng tiếp diễn: mobile thống trị, thanh toán di động (Apple Pay, Google Wallet, WeChat Pay), voice commerce, chatbot và AI/ML cho product recommendation và personalisation.

### Ví dụ thực tế
Tủ lạnh thông minh ([[IoT]]) có thể tự đặt lại thực phẩm sắp hết qua subscription với siêu thị — ví dụ về automated e-commerce không cần con người can thiệp, hướng đi giảm friction trong giao dịch.

### Liên kết
- [[Digital Business]] — e-commerce là tập con
- [[Mobile Commerce]], [[Social Commerce]], [[Livestreaming Commerce]]
- [[EDI]] — tiền thân của giao dịch điện tử (chi tiết ở [[CH06 - Digital Supply Chain Management]])

---

## Strategy for E-commerce (Chiến lược E-commerce)

### Định nghĩa (Definition)
Chiến lược e-commerce phải đặt trong khung digital business strategy (Chương 5), trả lời 2 câu hỏi cốt lõi: **e-commerce value proposition là gì?** (giá trị tạo ra cho khách hàng) và **revenue stream đến từ đâu?**

### Giải thích chi tiết
Năm [[Revenue Model]] phổ biến:
1. **Classic sales model** — doanh thu trực tiếp từ bán hàng hóa/dịch vụ;
2. **Advertising income model** — miễn phí cho người dùng, thu tiền nhà quảng cáo;
3. **[[Subscription Model]]** — trả phí định kỳ để truy cập;
4. **[[Freemium]]** — bản cơ bản miễn phí, thu phí bản premium;
5. **Transaction fee model** — thu phí trên mỗi giao dịch được thực hiện.
Kết hợp nhiều mô hình gọi là **hybrid revenue model** (Amazon với Prime + Marketplace + Ads là ví dụ điển hình).

Sáu **operating model** hiện hành: Retail (cửa hàng online kinh điển, rào cản gia nhập thấp), Content (Netflix, Spotify — rào cản cao vì chi phí sản xuất và bản quyền), Transactor (dịch vụ tài chính, [[FinTech]], share-dealing app, [[Online Travel Agents]]), Social network (Tinder, Bumble — thường freemium/subscription), [[Aggregator]] (gom cả cung và cầu, sống bằng quảng cáo/affiliate — các site so sánh giá) và [[Marketplace]] (eBay, Amazon — doanh số marketplace 2021 đạt **103 tỷ USD**; cuối 2022 chiếm **58% unit sales của Amazon**).

Năm operating model riêng cho [[B2B]] phản ánh bản chất chuỗi cung ứng: wholesale, procurement marketplace (Alibaba), private B2B procurement platform, private vertical và sector vertical.

**Phát triển platform**: bắt đầu từ ideation (mission, objectives, business model, target audience, channel choice); quản lý phát triển chuyển từ waterfall sang **agile** với vòng lặp cải tiến nhỏ; nền tảng dễ dùng (Shopify, Wix) cho phép thử nghiệm thị trường kiểu prototyping. Hai quyết định then chốt: ai **xây** platform ban đầu và ai **vận hành** lâu dài (in-house vs outsource cho agency chuyên Magento/Sitecore).

**[[Headless E-commerce]]**: tách rời (decouple) frontend và backend, thay thế nền tảng monolithic dạng silo. Mọi interface (web, app, store) truy cập cùng một bộ dữ liệu và service nhất quán; microservice (reviews, loyalty) có thể thêm vào và dùng chung. Lợi ích: giảm phức tạp, nhất quán đa kênh, future-proof khoản đầu tư backend, outsource từng frontend riêng lẻ.

**Payment systems**: thẻ vẫn lớn nhất nhưng lựa chọn tăng nhanh — WeChat Pay thống trị Trung Quốc; Google Pay/Apple Pay; PayPal; P2P payments (Monzo); [[Cryptocurrency]] (CheapAir.com, Virgin Galactic chấp nhận) dù độ tin cậy còn thấp; và **[[Buy Now Pay Later]]** (Klarna, Afterpay, Affirm) bùng nổ từ đại dịch — giảm friction với giỏ hàng giá trị cao, nhà cung cấp BNPL gánh rủi ro và thu phí vendor, nhưng bị chỉ trích vì đẩy nợ tiêu dùng không bảo đảm ra ngoài các quy chế tín dụng.

### Ví dụ thực tế
Cuối 2021 Amazon tranh chấp với Visa về phí giao dịch, từng ngừng chấp nhận thẻ Visa trước khi hai bên đạt thỏa thuận — minh họa transaction cost là biến số đàm phán được với vendor lớn, nhưng không co giãn với vendor nhỏ.

### Liên kết
- [[Revenue Model]], [[Freemium]], [[Subscription Model]]
- [[Headless E-commerce]], [[Buy Now Pay Later]]
- [[CH05 - Digital Business Strategy]] — khung chiến lược tổng thể
- [[CH02 - Opportunity Analysis]] — business model và marketplace analysis

---

## B2C and Retail E-commerce (B2C và bán lẻ trực tuyến)

### Định nghĩa (Definition)
[[B2C]] retail e-commerce là mảng lớn nhất và quen thuộc nhất: thị trường retail e-commerce toàn cầu dự kiến tăng từ **5.000 tỷ USD (2021) lên 7.000 tỷ USD (2025)** (Statista), với mobile chiếm **73% traffic** và **63% đơn hàng** (desktop lần lượt 25% và 35%).

### Giải thích chi tiết
Khoảng cách traffic–order cho thấy người dùng nghiên cứu trên mobile nhưng chốt đơn trên desktop, và khoảng cách này đang thu hẹp. Voice commerce tăng từ **4,6 tỷ USD (2021) lên dự kiến 19,4 tỷ (2023) và 99 tỷ USD (2026)**. Image search ngày càng quan trọng (⅓ người trưởng thành dùng thường xuyên); AR/VR bắt đầu chứng minh giá trị — Ingka Group (IKEA) dùng LiDAR trên iPhone scan phòng để đặt thử nội thất 3D, tăng conversion hàng giá trị cao và **giảm tỷ lệ trả hàng**.

Năm business model B2C phổ biến:
- **Single channel (pureplay)**: chỉ bán online (Ocado, Kogan.com) — rào cản gia nhập thấp nhưng cạnh tranh gay gắt, margin mỏng.
- **Catalogue evolvers**: doanh nghiệp catalogue truyền thống chuyển đổi (N Brown, Eddie Bauer, Pottery Barn) — chi phí cao hơn pureplay nhưng sở hữu sẵn hạ tầng kho vận.
- **Multi-channel ("bricks-and-clicks")**: tiến hóa từ retail offline (John Lewis, Walmart, Target, Woolworths).
- **[[D2C]] (Direct-to-Consumer)**: thương hiệu bán thẳng, bỏ qua [[Intermediary]] để cải thiện margin (Dollar Shave Club — Unilever mua 2016, Hims & Hers, Bonobos, Shein); rủi ro chính là **channel conflict** với nhà bán lẻ truyền thống.
- **[[Omnichannel]] experience**: khác multi-channel ở chỗ **hành trình khách hàng di chuyển giữa các kênh** trong cùng một giao dịch (mua online – nhận tại cửa hàng click-and-collect, trải nghiệm tại store – giao tận nhà).

**B2C service models**: dịch vụ là sản phẩm vô hình, e-commerce xóa yêu cầu đồng thời giữa nhà cung cấp và khách. Các vertical nổi bật: (1) [[FinTech]] — challenger banks (NuBank, Chime, WeBank, Monzo) nhờ deregulation và [[Open Banking]] (PSD2); aggregator tài chính (NerdWallet, CompareTheMarket) đẩy broker truyền thống ra rìa; account aggregator (app Snoop) gom mọi sản phẩm tài chính về một chỗ rồi bán chéo. (2) [[Online Travel Agents]] — Expedia, Booking.com, Agoda, Trip.com; sản phẩm nhạy cảm về giá nên OTA tập trung khác biệt hóa bằng gói cá nhân hóa; chịu disruption từ search engine và C2C (Airbnb). (3) **On-demand và local**: Uber, Deliveroo, DoorDash, Meituan, Instacart, Getir — bùng nổ trong lockdown nhờ vốn VC, rồi co cụm về các đô thị đông dân khi nhu cầu giảm; đối mặt vấn đề đạo đức về lao động gig economy.

### Ví dụ thực tế
Getir, Zapp, Jiffy, Gorillas tăng trưởng bùng nổ khi lockdown nhưng khi người tiêu dùng quay lại mua trực tiếp, order value nhỏ không gánh nổi chi phí giao hàng thực; hàng loạt bị mua lại hoặc sụp đổ — bài học về đánh giá nhu cầu thực và tính bền vững của business model hậu khủng hoảng.

### Liên kết
- [[D2C]], [[Omnichannel]], [[Intermediary]]
- [[FinTech]], [[Open Banking]], [[Online Travel Agents]]
- [[Case 3.1 Páramo]] — chiến lược 2 kênh tách biệt

---

## B2B E-commerce (Thương mại điện tử B2B)

### Định nghĩa (Definition)
[[B2B]] e-commerce là giao dịch điện tử giữa các tổ chức, gắn chặt với electronic supply chain management. Quy mô **vượt xa B2C**: doanh thu B2B marketplace toàn cầu đạt **130 tỷ USD năm 2022**, riêng Amazon Business chiếm ~**25 tỷ USD**.

### Giải thích chi tiết
Phân biệt với [[EDI]]: EDI phục vụ đặt hàng lặp lại, khối lượng lớn, tự động trong quan hệ sẵn có; B2B e-commerce phục vụ đặt hàng ad-hoc "as you need it" và quan hệ khách hàng mới — nhiều ứng dụng B2B nhúng sẵn năng lực EDI.

Quy trình procurement chuẩn: tìm supplier → qualify theo tiêu chí → đàm phán (spec, khối lượng, giá, điều khoản) → hợp đồng → purchase order → invoice → fulfilment → thanh toán. Hai loại mua hàng: nguyên liệu cho sản xuất và hàng hóa vận hành hằng ngày; hai hình thức: **call-off contract** (cam kết trước, giao dần) và **one-off purchase**.

Các loại marketplace B2B: buy-side (do tập đoàn mua sở hữu — Walmart quản lý hàng nghìn supplier qua buy-side marketplace), sell-side, B2B vertical (một ngành, ví dụ hàng không), B2B horizontal (một nhóm sản phẩm cho mọi ngành), sector portal do chính ngành sở hữu. Cấu trúc marketplace phản ánh **tương quan quyền lực buyer–supplier**.

Minh bạch chuỗi cung ứng ([[Supply Chain Visibility]]) cho phép JIT, lean production và tồn kho tinh gọn — nhưng Brexit, lockdown và "pingdemic" đã phơi bày rủi ro của chuỗi cung ứng quá lean, nhất là khi phụ thuộc supplier Trung Quốc; lean cũng bị phê phán về tác động môi trường khi vận chuyển xa.

### Ví dụ thực tế
Đại dịch buộc giao dịch B2B pivot nhanh sang e-commerce — nhưng thực chất chỉ tăng tốc xu hướng có sẵn, với động lực là giảm chi phí, tăng hiệu quả và productivity gain từ tự động hóa.

### Liên kết
- [[EDI]], [[e-Procurement]], [[Supply Chain Visibility]]
- [[CH06 - Digital Supply Chain Management]] — chi tiết e-procurement và SCM

---

## Content and Entertainment E-commerce (Nội dung và giải trí)

### Định nghĩa (Definition)
Content e-commerce giao dịch sản phẩm **vô hình**: tạo ra một lần nhưng bán và tiêu thụ hàng triệu lần — gồm video, audio, written materials (eBooks, báo chí) và gaming.

### Giải thích chi tiết
- **Video**: content distributor (Netflix, Prime Video, Tencent Video, iQIYI) đang tiến vào sản xuất nội dung; studio truyền thống (Paramount+, Disney+) đi ngược lại vào phân phối — thị trường phân mảnh dần, subscriber bắt đầu chọn lọc và hủy bớt dịch vụ.
- **Audio**: Spotify, Apple Music — dịch chuyển từ mua/download sang streaming theo subscription.
- **eBooks**: Amazon Kindle gần như thống trị; **news publishing** doanh thu kém vì người dùng quen nội dung miễn phí, "đổi eyeballs lấy content" qua quảng cáo hành vi.
- **Gaming**: từ console/hardware sang download, online gameplay, subscription (Fortnite 'Save the World'), mobile casual; Apple/Google giữ tới **30% in-app purchase**; **loot boxes** gây tranh cãi pháp lý — một số nước coi là cờ bạc không đăng ký.

Số liệu tiêu thụ: media qua mobile tăng từ 1h38'/ngày (2013) lên 3h36' (2020); trong lockdown UK 2020, tiêu thụ news tăng 32%, streaming live 48%, nội dung ghi sẵn 39%. Ba mô hình doanh thu: subscription, freemium/ad-supported (Spotify Free, Netflix Basic with Adverts), pay-per-view.

### Ví dụ thực tế
Netflix và Prime Video — vốn thuần subscription — phải mở gói "free" có quảng cáo để giữ thuê bao khi kinh tế bất ổn và số nhà cung cấp trả phí tăng vọt: minh chứng revenue model phải tiến hóa theo hành vi trả tiền của khách.

### Liên kết
- [[Revenue Model]], [[Freemium]], [[Subscription Model]]
- [[6 Digital Media Channels|Digital Media Channels]] — phối hợp với truyền thông ở [[CH08 - Digital Communications]]

---

## Marketplaces, Communities and Auctions (Marketplace, cộng đồng và đấu giá)

### Định nghĩa (Definition)
[[Marketplace]] và mạng xã hội đều **aggregate** khách hàng — mạng xã hội gom theo hành vi/địa lý/tâm lý, marketplace gom theo **nhu cầu hàng hóa và dịch vụ**.

### Giải thích chi tiết
Các kiểu aggregation trên mạng xã hội: single platform ("vì mọi người ở đó"), AIO psychographic (theo sở thích), owned community (Discourse/Slack/Discord của tổ chức), communities of practice (nghề nghiệp), cultural/beliefs-driven. Dù hấp dẫn, **social commerce chưa bùng nổ như dự đoán**: Facebook Shops chỉ giới hạn ở Mỹ và vẫn cần website e-commerce riêng; Pinterest, Twitter Shops chỉ là tích hợp trỏ về site ngoài; TikTok Shopping checkout trong app chỉ có ở Trung Quốc, một phần Đông Nam Á và UK. Ngoại lệ là Trung Quốc: WeChat **Mini-Programs** với WeChat Pay, TaoBao Live cho phép mua ngay trong livestream với KOL/KOC làm host — tạo niềm tin và tính chân thực văn hóa.

Lợi ích bán qua [[Marketplace]]: outsource rủi ro vận hành, thêm kênh tiếp cận, dùng hạ tầng logistics (Amazon FBA: kho, nhặt hàng, fulfilment), thống trị kết quả product search. Nhược điểm: phí cao nhiều tầng, sản phẩm copycat xuất hiện nhanh, và marketplace có thể dùng chính data của vendor để cạnh tranh — Reuters (2021) đưa tin Amazon Ấn Độ dùng dữ liệu hiệu suất nội bộ của third-party vendor để copy sản phẩm bán chạy và bán rẻ hơn.

Ba mô hình đấu giá: **forward auction** (giá lên — eBay), **reverse/Dutch auction** (giá xuống tới khi có người mua — phổ biến trong mua sắm chính phủ Mỹ), **double/Vickrey auction** (khớp cung cầu tìm điểm giá tối ưu). Ứng dụng: thanh lý tồn kho nhanh, khám phá giá thị trường cho hàng hiếm, tách kênh "on-sale" khỏi kênh full-price. Rủi ro: shill bidding (thổi giá), shield bidding (dìm giá), returns scam.

### Ví dụ thực tế
Google Shopping trông giống marketplace nhưng **không có giao dịch nào diễn ra trong hạ tầng Google** — bản chất là môi trường quảng cáo referral về site bán lẻ; tương tự Reserve with Google cho đặt bàn, vé, lịch hẹn.

### Liên kết
- [[Marketplace]], [[Aggregator]], [[Social Commerce]], [[Livestreaming Commerce]]
- Online Auction, [[Disintermediation]] — D2C né marketplace
- [[Case 3.1 Páramo]] — dùng eBay Storefront làm kênh xả hàng riêng

---

## Security Issues in E-commerce (Bảo mật trong E-commerce)

### Định nghĩa (Definition)
Giao dịch tài chính khiến e-commerce thành mục tiêu hấp dẫn của cybercrime. Thế lưỡng nan của doanh nghiệp: **bảo mật đủ chặt nhưng friction đủ thấp** — quá nhiều lớp bảo mật làm khách bỏ giỏ hàng, quá ít thì rủi ro cho cả doanh nghiệp lẫn khách.

### Giải thích chi tiết
Dữ liệu bị đánh cắp phổ biến nhất: số thẻ 16 chữ số kèm mã bảo mật 3 số, câu hỏi bảo mật, dữ liệu dải từ, thông tin đăng nhập ngân hàng/PayPal, danh tính cá nhân (hộ chiếu, ID), tài khoản đăng nhập mạng chung (Google/Apple/Facebook sign-in).

Các hình thức gian lận trực tiếp: **identity theft** (dùng phương thức thanh toán hợp pháp mua hàng gian lận); khách hàng gian lận qua **chargeback** với ngân hàng để nhận hàng miễn phí; **fraudulent use of cards** khi kẻ tấn công kiểm soát nạn nhân đủ sâu (chiếm điện thoại nhận 2FA) khiến hệ thống chống gian lận tinh vi nhất cũng thất bại; **triangulation fraud** — dùng thẻ trộm mua hàng nhỏ gửi về địa chỉ nạn nhân để "nuôi" hồ sơ, sau đó mua đơn lớn gửi về điểm nhận hộ.

**Magecart / web skimming**: hacker tiêm mã độc vào website để hút dữ liệu form checkout — nạn nhân gồm cả Ticketmaster (2018), British Airways, Warner Music, WooCommerce (2021), và Liquor Control Board of Ontario (2023).

### Ví dụ thực tế
Magecart ban đầu gắn với các site chạy Magento nhưng đã lan rộng mọi nền tảng — cho thấy bảo mật e-commerce là cuộc đua liên tục, không phải cấu hình một lần.

### Liên kết
- [[Privacy]] và pháp lý dữ liệu ở [[CH04 - Key Issues in the Digital Environment]]
- Thiết kế bảo mật hệ thống (SSL, PKI) ở [[CH09 - Digital Experience and Service Design]]

---

## Practical Development of E-commerce Platforms (Thực hành phát triển platform)

### Định nghĩa (Definition)
Khi khách đã đến site, trọng tâm chuyển từ acquisition sang **conversion**. Ba trục phát triển: trải nghiệm (experience), điều hướng (navigation) và khả năng được tìm thấy (findability).

### Giải thích chi tiết
**UX cơ bản**: video sản phẩm tăng conversion cho hàng cần cân nhắc nhiều — Google (2018) ghi nhận >50% shopper nói video giúp họ quyết định mua; review là [[Social Proof]] quan trọng nhất (gần như mọi khách đều đọc review; điểm trung bình 5/5 với ít reviewer lại gây **mất** lòng tin); FAQ từ user-generated content; hiển thị tồn kho rõ ràng (kèm tùy chọn "email khi có hàng lại").

**Navigation và categorisation**: menu phải theo cách khách hàng nghĩ, không theo developer; site search nổi bật kèm auto-complete; category page (product listing page) là taxonomy sản phẩm, **collections** là tập hợp curated theo chủ đề (Summer, Office) hoặc theo brand, có thể cố định hoặc theo mùa.

**[[Call To Action]]**: lệnh hành động kèm động cơ — giảm rủi ro ("Buy today and save 20%!"), khan hiếm có thật ("vé giữ trong 10 phút"), hoặc gắn với benefit (Dollar Shave Club: "Need a Smooth Shave? Try for £5"). CTA phải nhìn thấy được mà **không cần scroll**. Phân biệt **macro-conversion** (hoàn tất đơn, đăng ký subscription) và **micro-conversion** (xem product page, thêm vào giỏ, xem video) — micro giúp dự đoán macro nhưng không phải mục tiêu chính; đây là nền tảng của [[Conversion Rate Optimisation]].

**Best practice** then chốt:
- **Responsive**: Google index bản mobile trước; hàng giá trị cao cần trải nghiệm kép mobile-nghiên-cứu/desktop-chốt-đơn; B2B có thể desktop-first vì chu kỳ mua dài.
- **[[Trust Signals]]**: copy và ảnh chất lượng, review từ nền tảng uy tín, địa chỉ thực xác minh được, chính sách đổi trả rõ; **giữ lại review tiêu cực** cũng là tín hiệu tin cậy. FOMO chỉ nên dùng khi khan hiếm là thật.
- **Recommendation, [[Cross-selling]] và [[Upselling]]**: gợi ý thay thế giữ chân khách, "Complete the Look" bán chéo hàng bổ trợ, upsell bản cao cấp — tăng order size mà không tạo áp lực.
- **Minh bạch giá và phí**: chi phí ẩn lộ ra ở checkout là nguyên nhân lớn nhất của cart abandonment (nghiên cứu 2023); hiển thị ngưỡng freeship ("Spend another $25 to get free shipping"). Which? (2022) phát hiện **98% deal Black Friday tại UK có giá bằng hoặc rẻ hơn vào thời điểm khác trong năm**.
- **Fulfilment và payment**: hiển thị ngày giao sớm nhất, tồn kho tại cửa hàng gần; càng nhiều lựa chọn thanh toán (card, PayPal, Apple/Google Pay, BNPL) càng tăng conversion.

**SEO cho product page** — các thành phần quyết định [[SEO]] visibility:
| Thành phần | Yêu cầu |
|---|---|
| URL | phản ánh cấu trúc category, chứa key phrase chính |
| Title tag | 50–60 ký tự (≤70), key phrase đứng đầu — thành phần quan trọng nhất |
| Meta description | không ảnh hưởng ranking nhưng là "quảng cáo" quyết định click |
| H1 | tên sản phẩm chứa key phrase + qualifier cho [[Long Tail]] search |
| Product description | key phrase trong 150–200 từ đầu, H2 theo related keywords, ngôn ngữ cho người |
| Ảnh | filename có nghĩa, Alt-Text đầy đủ (đồng thời phục vụ [[Accessibility]]) |
| Internal links | topic cluster giữa product page và category |

Phân biệt **search intent**: commercial ("best outfits for summer" → nhắm bằng category/collection page) và transactional (query dài chứa model number → nhắm bằng product page). Lưu ý: >60% người tiêu dùng Mỹ tìm sản phẩm trên **Amazon trước** so với ~50% dùng search engine (Jungle Scout, 2022).

### Ví dụ thực tế
[[Accessibility]] không phải tùy chọn: người khiếm thị dùng screen reader; caption video, Alt Text, độ tương phản cao và điều hướng bàn phím tạo khác biệt lớn với chi phí nhỏ.

### Liên kết
- [[Conversion Rate Optimisation]], [[AB Testing|A/B Testing]] — đào sâu ở [[CH09 - Digital Experience and Service Design]]
- [[SEO]], [[Long Tail]], Search Intent
- [[Usability]], [[Accessibility]], [[Social Proof]], [[Trust Signals]]

---

## Tóm tắt chương (Summary)

1. [[E-commerce]] là tập con của [[Digital Business]], tập trung vào giao dịch online — mạnh nhất ở retail, travel, tài chính và B2B.
2. Thông tin dồi dào khiến so sánh dễ dàng → vị trí hiển thị trên [[Marketplace]], comparison site và Google Shopping trở nên sống còn.
3. Doanh nghiệp multichannel phải tích hợp online–offline (click-and-collect) hướng tới [[Omnichannel]].
4. Chiến lược e-commerce = value proposition khác biệt + tổ hợp [[Revenue Model]] (Amazon là hybrid: ads + on-demand + subscription + B2B).
5. B2B có 5 operating model riêng phản ánh bản chất chuỗi cung ứng.
6. [[Headless E-commerce]] tách frontend/backend giúp tích hợp linh hoạt các dịch vụ như [[Buy Now Pay Later]].
7. [[Social Commerce]] và [[Livestreaming Commerce]] hỗ trợ cầu và doanh số, nhưng ngoài Trung Quốc vẫn chưa đạt kỳ vọng.
8. Best practice thiết kế (navigation, CTA, trust signals, minh bạch giá, SEO) trực tiếp nâng conversion rate.
