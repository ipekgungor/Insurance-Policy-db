# Health Insurance Company Database Project

This SQL project represents the database of a health insurance company. The tables have been created according to the following requirements, using Oracle:

## Requirements

1. **Customer Information**:
   - Each customer has a name, surname, address, phone number, up-to-date health information, and a unique customer ID.

2. **Insurance Policy Limitations**:
   - A customer may not have more than one insurance policy.
   - Not all customers must have an insurance policy.
   - An insurance policy must belong to exactly one customer.

3. **Insurance Policy Details**:
   - An insurance policy has a policy date and a unique policy number.
   - Each insurance policy must be associated with one or more contracted institutions.

4. **Contracted Institutions**:
   - Each contracted institution may be associated with one or more insurance policies.
   - Contracted institutions include details such as institution name, address, phone number, treatment method, and a unique institution ID.

5. **Insurance Policy Types**:
   - A policy can be of two types: Premium or Standard.
     - **Premium** policies offer unlimited dental and eye treatments.
     - **Standard** policies offer one-time eye treatment.

6. **Employee Information**:
   - Company employees have a name, surname, address, phone number, a unique SSN, and an employee ID.
   - Employees are responsible for zero or more customers.
   - Each customer is assigned exactly one responsible employee.

7. **Discounts**:
   - The company offers a 10% discount to employees who are also customers.
   - The company offers a 15% discount to customers who were with the company last year.

## Usage

- **Tables**: Tables are created with the necessary attributes and relationships as described in the requirements.
- **Queries**: SQL queries are provided for various operations and data retrieval needs.

## Getting Started

To set up the database:

1. Ensure you have Oracle Database installed.
2. Create the tables by executing the provided SQL scripts.
3. Insert sample data into the tables using the provided SQL insert statements.

## Contact
- **Developer:** İpek Güngör
- **Email:** ipekgungor2001@gmail.com
- **GitHub Profile:** ipekgungor

