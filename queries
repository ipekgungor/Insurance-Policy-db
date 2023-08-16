1.	
select c.customer_name, c.customer_surname, c.up_to_date_health_information, p.unlimited_dental_treatment, p.unlimited_eye_treatment
from customer c, insurancepolicy i, premium p
where c.customer_id = i.customer_id
and i.policy_id = p.policy_id
and p.unlimited_eye_treatment like '%twice'

2.	 SUBQUERY
select c.customer_name, c.customer_surname, c.customer_address
from customer c, ınsurancepolıcy i
where i.customer_id = c.customer_id
and i.policy_id IN (select policy_id
                    from insurancepolicy
                    where policy_date like '%2015')
order by customer_address desc

3.	ORDER BY
select emp_id, emp_name, emp_surname, emp_address
from employee
order by emp_id

4.	JOIN
select c.customer_name, c.customer_surname, e.emp_name
from customer c
join employee e
on e.SSN = c.employee_ssn
where emp_name = 'James'

5.	GROUP BY
select COUNT(*), employee_ssn
from customer
group by employee_ssn
