<template>
  <div class="testimonials">
    <h1>Testimonials</h1>
    <p>Don't just take our word for it. Here's what our satisfied customers have to say: hello my name is sedrick te third</p>
    <div class="testimonial-container">
      <div class="testimonial" v-for="testimonial in testimonials" :key="testimonial.name">
        <p>{{ testimonial.message }}</p>
        <p>- {{ testimonial.name }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TestimonialsView',
  data() {
    return {
      testimonials: [
        {
          name: 'John Doe',
          message: 'I had a great experience working with this team. They were professional, efficient, and delivered high-quality results.'
        },
        {
          name: 'Jane Smith',
          message: 'I was impressed by their attention to detail and ability to understand my needs. I would highly recommend them to anyone.'
        },
        {
          name: 'Bob Johnson',
          message: 'Their communication skills are top-notch. They kept me informed throughout the entire process and exceeded my expectations.'
        }
      ]
    }
  }
}
</script>

<style scoped>
.testimonials {
  text-align: center;
  padding: 20px;
}

.testimonial-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.testimonial {
  margin: 20px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  width: 30%;
}

.testimonial p {
  margin-bottom: 10px;
}

.testimonial p:last-child {
  font-weight: bold;
  color: #337ab7;
}
</style>