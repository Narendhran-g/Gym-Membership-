
# Gym Membership Database - SQL Queries

This SQL script sets up a basic Gym Membership Database to track members, subscriptions, attendance, and more. The script includes the database schema, sample data insertion, and stored procedures for managing member subscriptions and attendance.

## Database Structure

1. **Members Table**
   - Stores information about the gym members.
   - Columns: MemberID, Name, Age, Gender, Phone, Email, JoinDate.

2. **MembershipPlans Table**
   - Stores different types of membership plans offered by the gym.
   - Columns: PlanID, PlanName, DurationMonths, Price.

3. **Subscriptions Table**
   - Stores the subscription details for each member, linking to both Members and MembershipPlans.
   - Columns: SubscriptionID, MemberID, PlanID, StartDate, EndDate.

4. **Attendance Table**
   - Tracks the attendance of members by recording check-in times.
   - Columns: AttendanceID, MemberID, CheckInTime.

## SQL Queries and Stored Procedures

1. **Creating Tables:**
   The script first creates the necessary tables for Members, MembershipPlans, Subscriptions, and Attendance.

2. **Inserting Sample Data:**
   Sample data is inserted into the Members, MembershipPlans, Subscriptions, and Attendance tables for demonstration.

3. **Stored Procedures:**
   - **Member_Subscriptions**: Retrieves all the subscriptions for each member, including plan names and start/end dates.
   - **Active_Members**: Finds members with subscriptions that are active from a specified date (e.g., today).
   
4. **Queries:**
   - **Get Member Subscriptions**: Displays member names, plan names, and subscription start/end dates.
   - **Active Members Query**: Retrieves active members whose subscriptions haven't expired.
   - **Last Check-In Time**: Finds the latest check-in time for each member.
   - **Most Frequent Check-In**: Retrieves the member with the most check-ins.
   - **Members Who Checked In Today**: Finds members who checked in today.
   - **Extend Subscription**: Extends a specific member's subscription by one month.
   - **Members with Subscription and Attendance**: Lists members who have both an active subscription and at least one check-in.

## How to Use

1. Execute the provided SQL script in a MySQL environment.
2. Use the stored procedures and queries to interact with the database and retrieve or manipulate data.

## License

This project is open-source and free to use.

