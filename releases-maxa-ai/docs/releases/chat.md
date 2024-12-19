# Chat - Release Notes

## Release Overview

Chat is a new chatbot product designed to help users interact with their data through a conversational interface.
Users can ask a variety of questions, from transactional inquiries like _"Give me the sales order line item details for sales order XXXX"_
to more complex business-related queries such as _"What were the total manufacturing labor costs and hours associated with project XXXX?"_.
Additionally, Chat offers question suggestions when further clarification is needed, aimed at enhancing the user's understanding and engagement with their data.

The chat currently references a limited number of marts the marts are as follows:

- `MART_SALES_ORDERS` _(PCR August logic)_
- `MART_PROJECTS_SUMMARY` _(PCR August logic)_
- `MART_NON_MANUFACTURING_LABOR_COSTS` _(PCR August logic)_
- `MART_MANUFACTURING_LABOR_COSTS` _(PCR August logic)_
- `MART_OTHER_COSTS` _(PCR August logic)_
- `MART_PRODUCTION_MATERIAL_COSTS` _(PCR August logic)_
- `EVENT_INTEGRATION_TRANSACTIONS_RECORDED` _(raw)_
- `EVENT_GL_TRANSACTIONS_LOGGED` _(raw)_
- `MART_MARGIN` _(tentative logic)_

:::warning **Important Note**
Chat QA is an experimental tool. While it aims to provide helpful and accurate responses, we cannot guarantee the accuracy of all answers…yet.
Please refer to the limitations section for more details on potential issues you may encounter.
We appreciate your understanding and feedback as we work to improve the product.
:::

## Key Features

### Conversational Query Interface

- **Ask Questions**: Easily input questions about your data using natural language.
  - _Example: Transactional Query_  
    "Provide sales order line item details for sales order 12345"
    <p align="center">
      <img src="/chat/image0.png" width="100%" />
    </p>
  - _Example: Business Query_  
    "What are the top 10 projects with the highest total actuals used?"
    <p align="center">
      <img src="/chat/image1.png" width="100%" />
    </p>

### SQL Query Visibility

- **See the SQL Queries:** For greater transparency and accuracy, Chat provides the option to see the SQL queries generated to answer your questions. This allows you to verify the logic behind the responses and ensure the results align with your expectations.
  - _Example: SQL Query Display_  
    When Chat provides a data answer, you can view the underlying SQL query for validation.
    <p align="center">
      <img src="/chat/image2.png" width="100%" />
    </p>

### Automated Suggestions

- **Question Suggestions**: Chat offers suggestions when additional information is required to provide a more accurate answer.
  - _Example: Clarification Needed_
    <p align="center">
      <img src="/chat/image3.png" width="100%" />
    </p>

### User Feedback and Improvement

- **Feedback Mechanism**: Share feedback on the quality of responses to help us improve Chat's accuracy and usability by clicking on the thumb icon and leaving a comment.
  <p align="center">
    <img src="/chat/image4.png" width="90%" />
    <p></p>
    <img src="/chat/image5.png" width="50%" />
  </p>

### Limitations

- **Intermittent Data Retrieval Issues**: Occasionally, Chat may respond that it couldn't find any information, even though the data is present. The same question, when asked again, might produce the correct results. This is a known limitation stemming from Cortex, the underlying LLM framework of our chatbot. At present, there is no standard method to predict or prevent this behaviour, and we advise reattempting queries when such instances arise.
- **Questions Clarity and Focus**:
  - **Clarity**: While natural language is supported, make technical aspects of your question clear when necessary. Include specific names for attributes and filter details to improve accuracy.
  - **Focused Requests**: Keep questions focused on a single task. Ask the chatbot to retrieve one query per mart to avoid confusion.
- **No Historical Context**: Chat treats each query independently. It doesn’t retain the context of previous questions from the same or earlier conversations, so always restate details necessary for the current query.
