# ACM_contest_website

# Upload Wordpress website to host
1. Login cPanel
2. File Manager -> Web Root (public_html/www) -> Domain -> Go
3. home/public_html -> upload -> upload file .ZIP
4. Extract file .ZIP

# Create database for host
1. Comeback to cPanel
2. MySQL Database
3. Create new database    [1]
4. Go Back
5. Create database user   [2]. (User [2.1], password [2.2])
6. Choose user [2] and database [1] -> Add -> All privileges
7. Comeback to cPanel
8. phpMyAdmin -> database [1] -> import -> file .SQL -> GO

#After completing the above steps, test run the web, FAIL. Right here, gg or do the steps below

# Editor file wp-config.php in public_html
1. Change database name in line "define( 'DB_NAME', ' [1] ' );
2. Change database user in line "define( 'DB_NAME', ' [2.1] ' );
1. Change database password in line "define( 'DB_NAME', ' [2.2] ' );

# Editor wp_options in phpMyAdmin
1. Change option value in "siteurl" and "home" to link domain
