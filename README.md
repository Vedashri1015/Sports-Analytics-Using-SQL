<h1>Sports Analytics Using SQL</h1>
        <p>
            This project explores IPL (Indian Premier League) cricket data using SQL to gain meaningful insights. 
            The analysis involves two datasets: one with match-level information and the other with ball-by-ball details. 
            This project is ideal for those looking to understand the role of SQL in sports analytics.
        </p>

<h2>Project Overview</h2>
        <p>
            As a sports analyst, you will import, organize, and analyze IPL datasets stored in a SQL database. 
            Key tasks include creating and modifying tables, querying data for insights, and summarizing results to answer specific questions about IPL matches and players.
        </p>

<h2>Datasets</h2>
        <ul>
            <li>
                <strong><code>IPL_matches.csv</code>:</strong>
                <ul>
                    <li>Contains data for 816 IPL matches from 2008 to 2020.</li>
                    <li>Includes details like match ID, date, teams, venue, winner, margin of victory, and player of the match.</li>
                </ul>
            </li>
            <li>
                <strong><code>IPL_Ball.csv</code>:</strong>
                <ul>
                    <li>Contains data for 193,468 balls bowled between 2008 and 2020.</li>
                    <li>Includes details like match ID, innings, overs, balls, batsmen, bowlers, runs, and dismissals.</li>
                </ul>
            </li>
        </ul>

<h2>SQL Tasks and Queries</h2>

<h3>Data Import and Table Creation</h3>
        <ol>
            <li>Create Tables:
                <ul>
                    <li><code>matches</code>: Match-level data.</li>
                    <li><code>deliveries</code>: Ball-by-ball data.</li>
                </ul>
            </li>
            <li>Import Data: Populate the tables using the provided CSV files.</li>
        </ol>

<h3>Basic Queries</h3>
        <ul>
            <li>Fetch top 20 rows from the <code>matches</code> and <code>deliveries</code> tables.</li>
            <li>Filter data based on specific conditions, such as matches played on a certain date, tied matches, or games with a margin of victory greater than 100 runs.</li>
        </ul>

<h3>Data Analysis Queries</h3>
        <ol>
            <li><strong>Count Analysis:</strong> Count the number of unique cities that have hosted IPL matches.</li>
            <li><strong>Table Enhancements:</strong> Create <code>deliveries_v02</code> with an additional column <code>ball_result</code>, categorizing balls as "boundary," "dot," or "other" based on runs scored.</li>
            <li><strong>Performance Metrics:</strong>
                <ul>
                    <li>Total boundaries and dot balls.</li>
                    <li>Boundaries scored and dot balls bowled by each team.</li>
                    <li>Dismissals grouped by dismissal type (excluding "NA").</li>
                    <li>Top 5 bowlers conceding the most extra runs.</li>
                </ul>
            </li>
            <li><strong>Venue Analysis:</strong>
                <ul>
                    <li>Total runs scored at each venue.</li>
                    <li>Year-wise runs scored at Eden Gardens.</li>
                </ul>
            </li>
        </ol>

<h3>Data Cleaning and Corrections</h3>
        <ul>
            <li>Create <code>matches_corrected</code> with standardized team names, replacing "Rising Pune Supergiants" with "Rising Pune Supergiant."</li>
            <li>Create <code>deliveries_v03</code> by adding venue and match date from the <code>matches</code> table to <code>deliveries_v02</code>.</li>
            <li>Generate <code>deliveries_v04</code> with a new column <code>ball_id</code> combining match ID, inning, over, and ball.</li>
        </ul>

<h3>Repetition Analysis</h3>
        <ul>
            <li>Use <code>row_number()</code> to identify and analyze repeating <code>ball_id</code> entries.</li>
        </ul>

<h2>Key Insights</h2>
        <ul>
            <li>Most boundaries scored by a team across IPL seasons.</li>
            <li>Cities with the highest number of IPL matches hosted.</li>
            <li>Teams with the most dot balls bowled.</li>
            <li>Bowlers contributing the most extra runs.</li>
            <li>Year-wise scoring patterns at specific venues.</li>
        </ul>

<h2>Skills Demonstrated</h2>
        <ul>
            <li><strong>Database Design:</strong> Table creation and data type selection.</li>
            <li><strong>Data Cleaning:</strong> Handling redundant or incorrect data.</li>
            <li><strong>Advanced SQL:</strong> Window functions (<code>row_number()</code>), subqueries, and conditional statements.</li>
            <li><strong>Data Analysis:</strong> Aggregations, filtering, and summarization.</li>
        </ul>

<h2>How to Use</h2>
        <ol>
            <li>Clone this repository and set up an SQL environment (MySQL, PostgreSQL, etc.).</li>
            <li>Import the datasets (<code>IPL_matches.csv</code> and <code>IPL_Ball.csv</code>) into the database.</li>
            <li>Execute the provided SQL queries to replicate the analysis.</li>
        </ol>

<h2>Potential Applications</h2>
        <ul>
            <li>Player performance analysis for fantasy leagues.</li>
            <li>Strategic insights for team managers.</li>
            <li>Venue-based scoring trends for sponsors and advertisers.</li>
        </ul>

<h2>Project Structure</h2>
        <ul>
            <li><strong>SQL Scripts:</strong> Contains all SQL queries used for analysis.</li>
            <li><strong>Data:</strong> Includes the datasets required for this project.</li>
            <li><strong>README:</strong> Project overview and instructions.</li>
        </ul>
