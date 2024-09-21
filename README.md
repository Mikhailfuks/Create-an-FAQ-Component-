<!DOCTYPE html>
<html>
<head>
  <title>FAQ Component</title>
  <style>
    .faq-container {
      width: 600px;
      margin: 0 auto;
      padding: 20px;
      border: 1px solid #ccc;
    }

    .faq-item {
      margin-bottom: 10px;
    }

    .faq-question {
      background-color: #f5f5f5;
      padding: 10px;
      cursor: pointer;
    }

    .faq-answer {
      padding: 10px;
      border: 1px solid #ccc;
      border-top: none;
      display: none; /* Hide answer initially */
    }
  </style>
</head>
<body>
  <div class="faq-container">
    <h2>Frequently Asked Questions</h2>

    <div class="faq-item">
      <div class="faq-question">What is your company's mission?</div>
      <div class="faq-answer">
        Our mission is to provide high-quality products and services that exceed customer expectations. 
      </div>
    </div>

    <div class="faq-item">
      <div class="faq-question">How do I contact customer support?</div>
      <div class="faq-answer">
        You can contact our customer support team via email at support@example.com or by phone at 1-800-555-1212.
      </div>
    </div>

    <!-- Add more FAQ items as needed -->

  </div>

  <script>
    const faqItems = document.querySelectorAll('.faq-item');

    faqItems.forEach(item => {
      const question = item.querySelector('.faq-question');
      const answer = item.querySelector('.faq-answer');

      question.addEventListener('click', () => {
        answer.style.display = answer.style.display === 'none' ? 'block' : 'none';
      });
    });
  </script>
</body>
</html>
