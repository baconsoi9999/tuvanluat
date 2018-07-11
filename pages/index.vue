<template>
<div>
  <Header/>
  <div class="container">
  <Slide/>
  <Info
    title="Giải pháp nào cho"
    subtitle="doanh nghiệp của bạn"
    text = "Tại Eazy Marketing, chúng tôi không bán quảng cáo mà tập trung tìm hiểu, tư vấn và cung cấp cho từng doanh nghiệp giải pháp phù hợp nhất theo từng thời điểm!

"
  />
  <InfoThumbnail/>
  <Info
    title="dự án tiêu biểu"
    text="Sự đam mê và tâm huyết với từng thương hiệu đã thôi thúc chúng tôi tạo nên những chiến dịch Marketing toàn diện và hiệu quả cao cho khách hàng của mình.

"
  />
  <ProjectInfo/>
  <Info
    title="KHÁCH HÀNG NÓI VỀ"
    subtitle="EAZY MARKETING"
    text="Di sản của Eazy Marketing là những lời khen tặng và góp ý từ những khách hàng đã sử dụng dịch vụ của chúng tôi. Đó chính là bằng chứng nhận quý giá và công bằng nhất

"
  />
  <Aboutus/>
  </div>
</div>
</template>

<script>
import Header from '~/components/Header/Header'
import Slide from '~/components/SlideShow/Slide'
import Info from '~/components/Info/Info'
import InfoThumbnail from '~/components/Info/InfoThumbnail'
import ProjectInfo from '~/components/Info/ProjectInfo'
import Aboutus from '~/components/Info/Aboutus'


export default {
  components: {
    Header,
    Slide,
    Info,
    InfoThumbnail,
    ProjectInfo,
    Aboutus
  }
}
</script>