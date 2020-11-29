<template>
  <table class="table table-bordered table-hover">
    <thead>
      <tr class="table-primary">
        <th scope="col">Task Action</th>
        <th scope="col">Type</th>
        <th scope="col">Internal</th>
        <th scope="col">Invoicing Type</th>
        <th scope="col">Author</th>
        <th scope="col">Date</th>
        <th scope="col" style="text-align:right">Hours</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Daily</th>
        <td>Internal Meeting</td>
        <td></td>
        <td>Not Invoicing</td>
        <td>JYOJA</td>
        <td>2020-08-08</td>
        <td style="text-align:right">00:30</td>
      </tr>
      <tr>
        <th scope="row">Daily</th>
        <td>Internal Meeting</td>
        <td></td>
        <td>Not Invoicing</td>
        <td>JYOJA</td>
        <td>2020-08-08</td>
        <td style="text-align:right">00:30</td>
      </tr>
      <tr class="table-light">
        <th scope="row" colspan="2">Total</th>
        <th scope="row" colspan="5" style="text-align:right">01:00</th>
      </tr>
    </tbody>
  </table>
</template>
<script>
export default {
  name: "DailyTasks",
};
</script>