# How to use ChatGPT API to build a chatbot for product recommendations with embeddings

![Cover image](https://d2pwmb8xsybju4.cloudfront.net/posts/2023/chatgpt-recommend-products-embeddings/linkedin_card.png "Cover image")

**Are you looking to build a chatbot that can recommend products to your customers based on their unique profile?**<br>
Here's a step-by-step guide that shows you how to build a chatbot using embeddings to match a user's profile with relevant products from a company's database.

---

## Outline

**1. Introduction to embeddings**

**2. Get OpenAI API keys**

**3. Create a product dataset**

**4. Create embeddings for product dataset**

**5. Create a customer profile dataset**

**6. Create embeddings for customer profile dataset**

**7. Create embeddings for customer chat message**

**8. Get previous purchase data similarities**

**9. Get product database similarities**

**10. Create ChatGPT API prompt**

**11. Create ChatGPT product recommendations**

---

## Here's what we'll use:

**1. OpenAI API 🤖**

**2. Python 🐍**

---

## Detailed walkthrough
Read blog post for a detailed walkthrough: https://norahsakal.com/blog/chatgpt-product-recommendation-embeddings

## Troubleshooting

### attributeError: module 'openai' has no attribute 'ChatCompletion'

This probably means that the version of your **Python client library for the OpenAI API** is lower than `0.27.0`.

Run `pip install openai --upgrade` in your terminal for the latest version and make sure it is at least `0.27.0`:

![Upgrade OpenAI package](https://d2pwmb8xsybju4.cloudfront.net/posts/2023/chatgpt-api/4_troubleshooting.png "Upgrade OpenAI package")

---

### InvalidRequestError: This model's maximum context length is 4096 tokens

This indicates that the input `message_object` sent to the ChatGPT API has exceeded the maximum allowed length of 4096 tokens.

You will need to shorten the length of your messages to resolve the issue:

![Upgrade OpenAI package](https://d2pwmb8xsybju4.cloudfront.net/posts/2023/chatgpt-api/5_troubleshooting_2.png "Upgrade OpenAI package")
