SELECT project_id, ROUND(AVG(experience_years), 2) AS average_years
<br>
FROM Project
<br>
LEFT JOIN Employee
<br>
ON Project.employee_id = Employee.employee_id
<br>
GROUP BY project_id;
