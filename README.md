<h2>Swiss Tournament Database</h2>
<p>A Python module that uses the PostgreSQL database to keep track of players and matches in a game tournament.</p>

<p>The game tournament will use the Swiss system for pairing up players in each round: players are not eliminated, and each player should be paired with another player with the same number of wins, or as close as possible.<p>

<ul>
	<li>Supports multiple tournaments. Players can be registered in more than one tournament at a time.</li>
	<li>Allows for an odd number of players in a tournament. If there is an odd number, then a randomly selected player receives a bye.</li>
	<li>Ties are allowed.</li>
	<li>Utilizes OMW system when two players have the same rank (byes count as a free win).</li>
</ul>

<h2>How to Run</h2>
Assumes Python and Postgres environment have been properly set up and the project folder has been copied.

<ol>
	<li>Navigate to the project folder</li>
	<li>Using psql, enter the following command to create the tournament database<br>
		<code>create database tournament</code></li>
	<li>Using psql, enter the following command to connect to the tournament database<br>
		<code>\c tournament</code></li>
	<li>Using psql, enter the following command to create the tables and views for the tournament database<br>
		<code>\i tournament.sql</code></li>
	<li>Exit psql. Using command line, enter the following command to run the test file<br>
		<code>python tournament_test.sql</code></li>
</ol>

<p>There are 12 tests that should pass successfully</p>
