// Back to Top Button Functionality
window.onscroll = function() {toggleBackToTopButton()};

function toggleBackToTopButton() {
    if (document.body.scrollTop > 200 || document.documentElement.scrollTop > 200) {
        document.getElementById("back-to-top").style.display = "block"; // Show the button
    } else {
        document.getElementById("back-to-top").style.display = "none"; // Hide the button
    }
}

// Function to smoothly scroll back to top when the button is clicked
function scrollToTop() {
    window.scrollTo({
        top: 0,
        behavior: 'smooth' // Smooth scrolling to the top
    });
}
