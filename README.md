# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sample Registration Page</title>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>Welcome to the Sample Registration Page</h1>
    </header>

    <!-- Ordered List with Roman Numerals -->
    <section>
        <h2>Steps to Register</h2>
        <ol type="I">
            <li>Fill in your personal details</li>
            <li>Choose a preferred subscription</li>
            <li>Submit the form</li>
        </ol>
    </section>

    <!-- External Image from Pexels -->
    <section>
        <h2>Our Beautiful Background</h2>
        <img src="https://images.pexels.com/photos/57008/pexels-photo-57008.jpeg" alt="Beautiful Scenery" width="500">
    </section>

    <!-- Table of 5 Contacts -->
    <section>
        <h2>Contact List</h2>
        <table border="1">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Address</th>
                    <th>Mobile</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>John Doe</td>
                    <td>123 Main St, City</td>
                    <td>(555) 123-4567</td>
                    <td>johndoe@example.com</td>
                </tr>
                <tr>
                    <td>Jane Smith</td>
                    <td>456 Oak Rd, Town</td>
                    <td>(555) 234-5678</td>
                    <td>janesmith@example.com</td>
                </tr>
                <tr>
                    <td>Mike Johnson</td>
                    <td>789 Pine Ln, Village</td>
                    <td>(555) 345-6789</td>
                    <td>mikejohnson@example.com</td>
                </tr>
                <tr>
                    <td>Emily Davis</td>
                    <td>101 Maple Ave, Suburb</td>
                    <td>(555) 456-7890</td>
                    <td>emilydavis@example.com</td>
                </tr>
                <tr>
                    <td>Chris Lee</td>
                    <td>202 Birch Blvd, City</td>
                    <td>(555) 567-8901</td>
                    <td>chrislee@example.com</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Registration Form -->
    <section>
        <h2>Register Here</h2>
        <form action="/submit" method="POST">
            <!-- Name Field -->
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter your full name" required><br><br>

            <!-- Email Field -->
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter your email" required><br><br>

            <!-- Password Field -->
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Enter your password" required><br><br>

            <!-- Date Field -->
            <label for="date">Date of Birth:</label>
            <input type="date" id="date" name="dob" required><br><br>

            <!-- Dropdown Field -->
            <label for="subscription">Subscription Plan:</label>
            <select id="subscription" name="subscription" required>
                <option value="basic">Basic</option>
                <option value="premium">Premium</option>
                <option value="vip">VIP</option>
            </select><br><br>

            <!-- Radio Buttons for Gender -->
            <fieldset>
                <legend>Gender:</legend>
                <input type="radio" id="male" name="gender" value="male">
                <label for="male">Male</label><br>
                <input type="radio" id="female" name="gender" value="female">
                <label for="female">Female</label><br>
                <input type="radio" id="other" name="gender" value="other">
                <label for="other">Other</label><br><br>
            </fieldset>

            <!-- Checkboxes for Interests -->
            <fieldset>
                <legend>Interests:</legend>
                <input type="checkbox" id="sports" name="interests" value="sports">
                <label for="sports">Sports</label><br>
                <input type="checkbox" id="music" name="interests" value="music">
                <label for="music">Music</label><br>
                <input type="checkbox" id="travel" name="interests" value="travel">
                <label for="travel">Travel</label><br><br>
            </fieldset>

            <!-- Submit Button -->
            <button type="submit">Submit Registration</button>
        </form>
    </section>

</body>
</html>
