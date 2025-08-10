<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Lost & Found Tracker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Lost & Found Tracker</h1>
        <p>Report, track, and recover lost items</p>
    </header>

    <main>
        <!-- Report Section -->
        <section id="report-section">
            <h2>Report Lost or Found Item</h2>
            <form id="report-form">
                <label>Item Type:
                    <select name="type" required>
                        <option value="lost">Lost</option>
                        <option value="found">Found</option>
                    </select>
                </label>
                <label>Item Name: <input type="text" name="name" required></label>
                <label>Description: <textarea name="description" rows="2"></textarea></label>
                <label>Location: <input type="text" name="location" required></label>
                <label>Date: <input type="date" name="date" required></label>
                <label>Image: <input type="file" name="image" accept="image/*"></label>
                <button type="submit">Submit</button>
            </form>
        </section>

        <!-- Search Section -->
        <section id="search-section">
            <h2>Search Items</h2>
            <input type="text" id="search-bar" placeholder="Search by name, location...">
            <div id="item-list"></div>
        </section>
    </main>

    <footer>
        <p>Lost & Found Tracker — Demo</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
