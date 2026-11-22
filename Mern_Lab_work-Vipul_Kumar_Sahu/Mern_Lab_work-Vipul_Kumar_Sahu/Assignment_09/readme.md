1. Experiment Title
Tables with Headers and Footers
2. Aim
Create marks tables with captions, header/body/footer sections, averages, and scope attributes.
3. Software / Tools Required
VS Code or text editor, web browser
4. Theory
HTML tables organize tabular data using table, caption, thead, tbody, tfoot, tr, th, and td. scope=col and scope=row help assistive technology associate cells with headers. Average is the sum divided by the number of values.
5. Algorithm / Procedure
35.	Create marks.html with caption, header, and four student rows (Vipul, Ansh, Harikesh, Ravi).
36.	Create marks-average.html with Vipul, Ansh, Harikesh, and Ravi and calculate each subject average.
37.	Create marks-accessible.html with scope=col on column headers and scope=row on name headers.
6. Program / Queries / Commands
marks.html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Marks of Class A</title></head>
<body>
<table border="1">
  <caption>Marks of Class A</caption>
  <thead><tr><th>Name</th><th>Maths</th><th>Science</th></tr></thead>
  <tbody>
    <tr><td>Vipul</td><td>92</td><td>89</td></tr>
    <tr><td>Ansh</td><td>84</td><td>82</td></tr>
    <tr><td>Harikesh</td><td>78</td><td>85</td></tr>
    <tr><td>Ravi</td><td>88</td><td>90</td></tr>
  </tbody>
</table>
</body>
</html>

marks-average.html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Marks Average</title></head>
<body>
<table border="1">
  <caption>Marks of Class A</caption>
  <thead><tr><th>Name</th><th>Maths</th><th>Science</th></tr></thead>
  <tbody>
    <tr><td>Vipul</td><td>92</td><td>89</td></tr>
    <tr><td>Ansh</td><td>84</td><td>82</td></tr>
    <tr><td>Harikesh</td><td>78</td><td>85</td></tr>
    <tr><td>Ravi</td><td>88</td><td>90</td></tr>
  </tbody>
  <tfoot><tr><th>Class average</th><td>85.5</td><td>86.5</td></tr></tfoot>
</table>
</body>
</html>

marks-accessible.html
<!DOCTYPE html>
<html lang="en">
<head><meta charset="UTF-8"><title>Accessible Marks</title></head>
<body>
<table border="1">
  <caption>Marks of Class A</caption>
  <thead><tr><th scope="col">Name</th><th scope="col">Maths</th><th scope="col">Science</th></tr></thead>
  <tbody>
    <tr><th scope="row">Vipul</th><td>92</td><td>89</td></tr>
    <tr><th scope="row">Ansh</th><td>84</td><td>82</td></tr>
    <tr><th scope="row">Harikesh</th><td>78</td><td>85</td></tr>
    <tr><th scope="row">Ravi</th><td>88</td><td>90</td></tr>
  </tbody>
</table>
</body>
</html>

7. Input
Marks: Vipul 92/89, Ansh 84/82, Harikesh 78/85, Ravi 88/90. Averages: Maths 85.5, Science 86.5.
8. Output
Tables show the specified rows; average footer shows 85.5 and 86.5; accessible table headers carry scope attributes.
Output screenshot: Insert a browser/terminal screenshot here after running the experiment.
9. Result
The experiment 'Tables with Headers and Footers' was completed successfully. The required concepts and tasks were implemented and verified using the stated tools.
10. Viva-Voce Questions
•	What is the purpose of caption?
•	Why use thead and tbody?
•	What do scope=col and scope=row mean?
