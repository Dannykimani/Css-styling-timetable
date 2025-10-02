<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Class Timetable</title>
  <style>
    /* ========== Reset ========== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* ========== Variables ========== */
    :root {
      --primary: #3498db;
      --secondary: #2ecc71;
      --break: #f39c12;
      --header: #34495e;
      --text: #fff;
      --hover: #2980b9;
      --active: #1abc9c;
    }

    /* ========== Layout ========== */
    body {
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      padding: 20px;
      display: flex;
      justify-content: center;
    }

    .container {
      max-width: 100%;
      overflow-x: auto;
    }

    h1 {
      text-align: center;
      margin-bottom: 20px;
      color: var(--header);
    }

    /* ========== Table Styles ========== */
    table {
      border-collapse: collapse;
      width: 100%;
      min-width: 900px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    thead th {
      background: var(--header);
      color: var(--text);
      padding: 12px;
      text-align: center;
    }

    tbody td {
      border: 1px solid #ddd;
      text-align: center;
      padding: 14px;
      min-width: 130px; /* Refusha box */
      transition: all 0.3s ease;
      font-style: italic; /* words ziwe zimeinama */
    }

    tbody td.break {
      background: var(--break);
      color: white;
      font-weight: bold;
    }

    /* Hover & Active states */
    tbody td:hover {
      background: var(--hover);
      color: #fff;
      cursor: pointer;
      transform: scale(1.03);
    }

    tbody td:active {
      background: var(--active);
      color: #fff;
      transform: scale(0.98);
    }

    /* Focus state (ukitumia tab) */
    tbody td:focus {
      outline: 3px solid var(--primary);
      box-shadow: 0 0 6px var(--primary);
    }

    /* Responsive */
    @media (max-width: 768px) {
      table {
        font-size: 14px;
      }
      tbody td {
        min-width: 100px;
        padding: 10px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Class Timetable</h1>
    <table>
      <thead>
        <tr>
          <th>Day</th>
          <th>8:00 - 9:00</th>
          <th>9:00 - 10:00</th>
          <th>10:00 - 11:00</th>
          <th>11:00 - 12:00</th>
          <th>12:00 - 1:00</th>
          <th>1:00 - 2:00</th>
          <th>2:00 - 3:00</th>
          <th>3:00 - 4:00</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Monday</td>
          <td><em>Form Tutorus Time</em></td>
          <td><em>Mathematics</em></td>
          <td><em>English</em></td>
          <td><em>Physics</em></td>
          <td class="break"><em>Lunch</em></td>
          <td><em>Chemistry</em></td>
          <td><em>Biology</em></td>
          <td><em>Business</em></td>
        </tr>
        <tr>
          <td>Tuesday</td>
          <td><em>Form Tutorus Time</em></td>
          <td><em>Kiswahili</em></td>
          <td><em>Mathematics</em></td>
          <td><em>Geography</em></td>
          <td class="break"><em>Lunch</em></td>
          <td><em>CRE</em></td>
          <td><em>Computer Studies</em></td>
          <td><em>English</em></td>
        </tr>
        <tr>
          <td>Wednesday</td>
          <td><em>Form Tutorus Time</em></td>
          <td><em>History</em></td>
          <td><em>Chemistry</em></td>
          <td><em>Biology</em></td>
          <td class="break"><em>Lunch</em></td>
          <td><em>Mathematics</em></td>
          <td><em>Physics</em></td>
          <td><em>English</em></td>
        </tr>
        <tr>
          <td>Thursday</td>
          <td><em>Form Tutorus Time</em></td>
          <td><em>CRE</em></td>
          <td><em>Kiswahili</em></td>
          <td><em>Business</em></td>
          <td class="break"><em>Lunch</em></td>
          <td><em>Mathematics</em></td>
          <td><em>Geography</em></td>
          <td><em>Physics</em></td>
        </tr>
        <tr>
          <td>Friday</td>
          <td><em>Form Tutorus Time</em></td>
          <td><em>English</em></td>
          <td><em>Biology</em></td>
          <td><em>Mathematics</em></td>
          <td class="break"><em>Lunch</em></td>
          <td><em>Chemistry</em></td>
          <td><em>Kiswahili</em></td>
          <td><em>Business</em></td>
        </tr>
      </tbody>
    </table>
  </div>
</body>
</html>
