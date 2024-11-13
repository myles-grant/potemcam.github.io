---
layout: minimal
title:  "Applications Dashboard"
blurb: "Welcome to the applications dashboard."

enterprise: true
company-subscription: true
control-panel: true
authenticated: true


---
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.datatables.net/1.11.5/js/jquery.dataTables.min.js"></script>
<style>
.table-container {
display: flex;
justify-content: space-around;
width: 100%;
margin-top: 20px;
}
.data-table {
width: 45%;
}
</style>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>


<!-- Start Hero Area -->
<section id="hero-area" class="hero-area admin-invisible hidden">
<!-- Single Slider -->
<div class="hero-inner">
    <div class="container">
	<div class="row ">
	    <div class="col-lg-6 co-12">
		<div class="home-slider">
		    <div class="hero-text">
			<h3 class="wow fadeInUp" data-wow-delay=".3s" style="visibility: visible; animation-delay: 0.3s; animation-name: fadeInUp;">Admin Console</h3>
			<h1 class="wow fadeInUp" data-wow-delay=".5s" style="visibility: visible; animation-delay: 0.5s; animation-name: fadeInUp;">Please Log In</h1>
			<p class="wow fadeInUp" data-wow-delay=".7s" style="visibility: visible; animation-delay: 0.7s; animation-name: fadeInUp;">Never miss a match.</p>



<div class="button wow fadeInUp" data-wow-delay=".9s" style="visibility: visible; animation-delay: 0.9s; animation-name: fadeInUp;">
			    <span href="http://www.twitter.com/scrumtuous" class="btn primary"><i class="lni lni-alarm"></i> Metrics Dashboard</span>
								<span href="https://github.com/scrumtuous" class="btn"><i class="lni lni-wallet"></i>Admin Panel</span>
			</div>
		    </div>
		</div>
	    </div>
	    <div class="col-lg-6 col-12">
		<div class="hero-image">
		    <div class="waves-block">
			<div class="waves wave-1"></div>
			<div class="waves wave-2"></div>
		    </div>
		    <img src="assets/images/phone.png" alt="#">
		</div>
	    </div>
	</div>
    </div>
</div>
<!--/ End Single Slider -->
</section>
<!--/ End Hero Area -->










<section id="testimonials" class="section testimonials style2 admin-visible">
        <div class="container">
  <div class="row">
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="dailySignups" width="300" height="250"></canvas>
    </div>
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="opportunityNotifications" width="300" height="250"></canvas>
    </div>
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="opportunityMatches" width="300" height="250"></canvas>
    </div>
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="timeOnPage" width="300" height="250"></canvas>
    </div>
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="siteVisitors" width="300" height="250"></canvas>
    </div>
    <div class="col-lg-4 col-md-6 mb-4">
      <canvas id="countryOfOrigin" width="300" height="250"></canvas>
    </div>
  </div>

<div class="row">
    <!-- Feedback By App Table -->
    <div class="col-lg-6 mb-4">
      <h4>Feedback By App</h4>
      <table id="feedbackByApp" class="display table table-striped table-bordered">
        <thead>
          <tr>
            <th>App Name</th>
            <th>Submitter</th>
            <th>Ranking</th>
            <th>Received Date</th>
            <th>Completion Status</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>Notifications</td><td>J. Doe</td><td>7</td><td>01/10</td><td style="color: green;">Complete</td></tr>
          <tr><td>Opportunities</td><td>M. Lee</td><td>5</td><td>02/15</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>Website</td><td>A. Fox</td><td>9</td><td>03/01</td><td style="color: green;">Complete</td></tr>
          <tr><td>General</td><td>K. Roe</td><td>3</td><td>04/05</td><td style="color: red;">Pending</td></tr>
          <tr><td>Notifications</td><td>S. Kay</td><td>6</td><td>05/18</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>Opportunities</td><td>R. Poe</td><td>8</td><td>06/22</td><td style="color: green;">Complete</td></tr>
          <tr><td>Website</td><td>B. Jae</td><td>4</td><td>07/09</td><td style="color: red;">Pending</td></tr>
          <tr><td>General</td><td>H. Doe</td><td>2</td><td>08/12</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>Notifications</td><td>T. Fox</td><td>10</td><td>09/21</td><td style="color: green;">Complete</td></tr>
          <tr><td>Opportunities</td><td>Y. Poe</td><td>1</td><td>10/30</td><td style="color: red;">Pending</td></tr>
        </tbody>
      </table>
    </div>

    <!-- Feedback Status Table -->
    <div class="col-lg-6 mb-4">
      <h4>Feedback Status</h4>
      <table id="feedbackStatus" class="display table table-striped table-bordered">
        <thead>
          <tr>
            <th>App Name</th>
            <th>Submitter</th>
            <th>Ranking</th>
            <th>Received Date</th>
            <th>Completion Status</th>
          </tr>
        </thead>
        <tbody>
          <tr><td>Website</td><td>P. Kay</td><td>7</td><td>01/02</td><td style="color: green;">Complete</td></tr>
          <tr><td>General</td><td>D. Roe</td><td>5</td><td>02/07</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>Notifications</td><td>G. Poe</td><td>9</td><td>03/14</td><td style="color: green;">Complete</td></tr>
          <tr><td>Opportunities</td><td>L. Fox</td><td>3</td><td>04/18</td><td style="color: red;">Pending</td></tr>
          <tr><td>General</td><td>C. Doe</td><td>6</td><td>05/20</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>Notifications</td><td>N. Lee</td><td>8</td><td>06/25</td><td style="color: green;">Complete</td></tr>
          <tr><td>Opportunities</td><td>Q. Jae</td><td>4</td><td>07/11</td><td style="color: red;">Pending</td></tr>
          <tr><td>Website</td><td>V. Poe</td><td>2</td><td>08/13</td><td style="color: orange;">In Progress</td></tr>
          <tr><td>General</td><td>U. Doe</td><td>10</td><td>09/19</td><td style="color: green;">Complete</td></tr>
          <tr><td>Notifications</td><td>Z. Kay</td><td>1</td><td>10/28</td><td style="color: red;">Pending</td></tr>
        </tbody>
      </table>
    </div>
  </div>

            <div class="row">
                <div class="col-12">
                    <div class="section-title style2">
                        <span>Applications Dashboard</span>
                        <h2>Control Panel</h2>
                        <p>Welcome to your control panel.</p>
                    </div>
                </div>
            </div>
            <div class="row">
                
{% for page in site.pages %}
  {% if page.path contains 'apps/' and page.control-panel %}
    <div class="col-lg-4 col-md-6 col-12">
  
      <div class="single-testimonial">
        <div class="top-section">

          {% assign show_default_icon = true %}

          {% if page.authenticated %}
              <i class="lni lni-lock" title="Authentication Required"></i>
              {% assign show_default_icon = false %}
          {% endif %}

          {% if page.control-panel %}
              <i class="lni lni-cog" title="Control Panel"></i>
              {% assign show_default_icon = false %}
          {% endif %}

          {% if page.subscription-product %}
              <i class="lni lni-user" title="Personal Subscription Required"></i>
              {% assign show_default_icon = false %}
          {% endif %}

          {% if page.corporate-subscription %}
              <i class="lni lni-network" title="Corporate Subscription Required"></i>
              {% assign show_default_icon = false %}
          {% endif %}

          {% if page.enterprise %}
              <i class="lni lni-apartment" title="Enterprise Access Required"></i>
              {% assign show_default_icon = false %}
          {% endif %}

          {% if show_default_icon %}
              <i class="lni lni-world" title="All Access"></i>
          {% endif %}

          <h3><a href="{{ page.url }}">{{ page.title }}</a></h3>
        </div>
        <p>{{ page.blurb }}</p>
      </div>

    </div>
  {% endif %}
{% endfor %}
               
                
            </div>
        </div>
    </section>

<script>
  // Helper function to generate random data within a range
  function getRandomData(num, min, max) {
    return Array.from({ length: num }, () => Math.floor(Math.random() * (max - min + 1)) + min);
  }

  // 1. Daily Sign-ups Chart
  new Chart(document.getElementById('dailySignups'), {
    type: 'line',
    data: {
      labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
      datasets: [{
        label: 'Daily Sign-ups',
        data: getRandomData(7, 10, 50),
        borderColor: 'rgba(75, 192, 192, 1)',
        backgroundColor: 'rgba(75, 192, 192, 0.2)',
        fill: true
      }]
    },
    options: { responsive: true }
  });

  // 2.  Notifications Per Day
  new Chart(document.getElementById('opportunityNotifications'), {
    type: 'bar',
    data: {
      labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
      datasets: [{
        label: 'Opportunity Notifications Sent',
        data: getRandomData(7, 20, 100),
        backgroundColor: 'rgba(153, 102, 255, 0.6)',
      }]
    },
    options: { responsive: true }
  });

  // 3. Opportunity Matches Found
  new Chart(document.getElementById('opportunityMatches'), {
    type: 'bar',
    data: {
      labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
      datasets: [{
        label: 'Opportunity Matches Found',
        data: getRandomData(7, 10, 50),
        backgroundColor: 'rgba(255, 159, 64, 0.6)',
      }]
    },
    options: { responsive: true }
  });

  // 4. Time on Page (in seconds)
  new Chart(document.getElementById('timeOnPage'), {
    type: 'line',
    data: {
      labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
      datasets: [{
        label: 'Time on Page (seconds)',
        data: getRandomData(7, 30, 300),
        borderColor: 'rgba(54, 162, 235, 1)',
        backgroundColor: 'rgba(54, 162, 235, 0.2)',
        fill: true
      }]
    },
    options: { responsive: true }
  });

  // 5. Site Visitors
  new Chart(document.getElementById('siteVisitors'), {
    type: 'line',
    data: {
      labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
      datasets: [{
        label: 'Site Visitors',
        data: getRandomData(7, 100, 1000),
        borderColor: 'rgba(255, 99, 132, 1)',
        backgroundColor: 'rgba(255, 99, 132, 0.2)',
        fill: true
      }]
    },
    options: { responsive: true }
  });

  // 6. Country of Origin (Pie Chart)
new Chart(document.getElementById('countryOfOrigin'), {
  type: 'bar',
  data: {
    labels: ['USA', 'Canada', 'UK', 'Germany', 'India'],
    datasets: [{
      label: 'Country of Origin',
      data: getRandomData(5, 10, 300),
      backgroundColor: [
        'rgba(255, 99, 132, 0.6)',
        'rgba(54, 162, 235, 0.6)',
        'rgba(255, 206, 86, 0.6)',
        'rgba(75, 192, 192, 0.6)',
        'rgba(153, 102, 255, 0.6)'
      ]
    }]
  },
  options: {
    indexAxis: 'y',  // Makes the bar chart horizontal
    responsive: true,
    scales: {
      x: {
        beginAtZero: true
      }
    }
  }
});
</script>
<script>
  // Initialize DataTables for both tables
  $(document).ready(function() {
    $('#serviceTickets').DataTable({
      paging: false,
      searching: false,
      info: false
    });
    $('#feedbackTickets').DataTable({
      paging: false,
      searching: false,
      info: false
    });
  });
</script>

