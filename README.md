<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ticket Booking Form</title>
    <!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-LT5FTJSYNY"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-LT5FTJSYNY');
</script>
    <link
        href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Montserrat:wght@400;700&display=swap"
        rel="stylesheet">
        <link rel="icon" type="image/x-icon" href="https://bingocircus.co.in/wp-content/uploads/2024/09/cropped-BC-Logo-PNG.png">
        
    <style>       
*{
   
    font-family: 'Roboto';
   box-sizing: border-box;
   
}
body {
   font-family: 'Arial', sans-serif;
   background-color: #f9f9f9;
   margin: 0;
   display: flex;
   justify-content: center;
   align-items: center;
   min-height: 100vh;
   

}


.header {
   display: flex;
   align-items: center;
   justify-content: center;
   margin: 15px;
}

.header h1 {
   color: #ED1B24;
   margin-top: 3px;
   font-size: 26px;
   font-family: 'Montserrat';
}

.header p {
   color: #2F3098;
   font-size: 18px;
   margin-top: -7px;
   font-weight: 600;
   font-family: 'Montserrat';
}

.form-container {
   box-shadow: 1px 4px 9.5px 0px rgba(0, 0, 0, 25%);
   border-radius: 20px;
   width: 750px;
   display: flex;
   flex-direction: column;
   align-items: center;
   justify-content: flex-start;
   gap: 20px;
   overflow: auto;
   position: relative;
}

.form-container h4 {
   text-align: center;
   margin: 20px 0;
   font-weight: bolder;
   font-size: 18px;
}


.row-container {
   display: flex;
   width: 100%;
   gap: 20px;
}

.container {
   width: 350px;
   background-color: #f9f9f9;
   display: flex;
   flex-direction: column;
   justify-content: flex-start;
   align-items: left;
}

.pay-container {
   display: flex;
   justify-content: space-between;
   box-shadow: 1px 1px 7.800000190734863px 1px rgba(0, 0, 0, 25%);
   gap: 35px;
   margin-top: 30px;
   padding: 10px;
   border-radius: 10px;
}

.logo img {
   width: 80px;
   margin: 10px;
}

label {
   display: flex;
   justify-content: left;
   align-items: left;
   padding: 8px;
   padding-left: 0px;
   font-size: 16px;
   color: #000;
   font-weight: bold;
   margin-bottom: 5px;
   font-family: 'Roboto';

}

input {
   background-color: #FFFFFF;
   width: 94.4%;
   padding: 21px;
   height: 22px;
   border: 1px solid #A4A4A4;
   border-radius: 8px;
   color: #000;
   font-size: 12px;
   font-weight: 100;
   font-family: 'Roboto';
}

select {
   background-color: #FFFFFF;
   color: #000;
   width: 100%;
   padding: 10px;
   height: 43px;
   border: 1px solid #A4A4A4;
   border-radius: 8px;
   font-size: 12px;
   cursor: pointer;
}

.time-btn.active {
   background-color: darkblue;
   color: white;
}

.time-btn:hover {
   transform: scale(1.07);
}

.time-options {
   display: flex;
   justify-content: space-between;
}

.time-btn:disabled {
   background-color: #d3d3d3;
   color: #ffffff;
   cursor: not-allowed;
   border: 1px solid #A4A4A4;

}

.time-btn {
   background-color: #ffffff;
   color: rgb(0, 0, 0);
   padding: 10px 15px;
   border: 1px solid #A4A4A4;
   border-radius: 8px;
   margin: 5px;
   cursor: pointer;
   font-family: 'Roboto';
   transition: background-color 0.3s ease, transform 0.3s ease;
}

.quantity-container {
   display: flex;
   align-items: center;
   justify-content: space-between;
}

.quantity-input {
   width: 30%;
   text-align: center;
   padding: 15px;
   font-size: 14px;
   border: 1px solid #A4A4A4;
   border-radius: 8px;
   font-family: 'Roboto';
   color: #000;
}

.quantity-container button {
   width: 60px;
   height: 32px;
   font-size: 24px;
   background: #2E2F89;
   color: white;
   border: none;
   border-radius: 8px;
   cursor: pointer;
   transition: background-color 0.3s ease, transform 0.3s ease;
}

.quantity-container button:hover {
   transform: scale(1.025);
}

.category-btn {
   display: block;
   margin: 5px 0;
   padding: 10px;
   width: 100%;
   border: 1px solid #A4A4A4;
   border-radius: 5px;
   background: #fff;
   cursor: pointer;
   font-family: 'Roboto';
   transition: background-color 0.3s ease, transform 0.3s ease;
}

.category-btn:hover {
   transform: scale(1.025);
}

.category-btn.active {
   background: #2E2F89;
   color: white;
   border: 1px solid #2E2F89;
}

.info-text {
   font-size: 16px;
   color: #555;

   text-align: left;
}

.summary {
   margin: 15px 0;
   font-weight: bold;
   font-size: 16px;
}

.btn-proceed {
   background-color: #42DA5D;
   color: white;
   padding: 10px;
   width: 170px;
   border: none;
   border-radius: 10px;
   font-size: 16px;
   cursor: pointer;
   font-family: 'Roboto';
   transition: background-color 0.3s ease, transform 0.3s ease;
}

.btn-proceed:hover {
   transform: scale(1.05);
}

.total-amount {
   text-align: left;
   font-size: 18px;
   margin-left: 5px;
   font-weight: 500;
}

.total-amount .quantity-display {
   font-size: 14px;
   text-align: left;
}

.payment-logos {
   margin-top: 0;
   display: flex;
   justify-content: center;
   gap: 20px;
}

.payment-logos img {
   height: 75px;
}

.error {
            display: flex;
            justify-content: left;
            color: red;
            text-align: left;
            font-size: 16px;
        }

@media (max-width: 768px) {
   body {
       padding: 0;
   }

   .form-container {
       display: flex;
       width: 100%;
       padding: 15px;
       justify-content: center;
       align-items: center;
       margin-bottom: 80px;
   }

   .main {
       padding: 0px;
       width: 100%;
       height: auto;

   }

   input {
       background-color: #FFFFFF;
       width: 99.4%;
       padding: 25px;
       height: 22px;
       border: 1px solid #A4A4A4;
       border-radius: 8px;
       color: #000;
       font-size: 16px;
       font-weight: 100;
   }
   select {
       background-color: #FFFFFF;
       color: #000;
       width: 100%;
       padding: 15px;
       height: auto;
       border: 1px solid #A4A4A4;
       border-radius: 8px;
       font-size: 16px;
       cursor: pointer;
   }
   .time-btn {
       background-color: #ffffff;
       color: rgb(0, 0, 0);
       padding: 14px 15px;
       border: 1px solid #A4A4A4;
       border-radius: 8px;
       font-size: 16px;
       margin: 5px;
       cursor: pointer;
       transition: background-color 0.3s ease, transform 0.3s ease;
   }
   .category-btn {
       display: block;
       margin: 5px 0;
       padding: 15px;
       font-size: 16px;
       width: 100%;
       border: 1px solid #A4A4A4;
       border-radius: 8px;
       background: #fff;
       cursor: pointer;
       transition: background-color 0.3s ease, transform 0.3s ease;
   }
   .quantity-input {
       width: 30%;
       text-align: center;
       padding: 25px;
       font-size: 18px;
       border: 1px solid #A4A4A4;
       border-radius: 8px;
       color: #000;
   }
   
   .quantity-container button {
       display: flex;
      padding: 25px;
      align-items: center;
      justify-content: center;
   }
   .container {
       width: 100%;
   }

   .row-container {
       width: 100%;
       display: flex;
       gap: 10px;
       flex-direction: column;
       align-items: center;


   }

   .pay-container {
       display: flex;
       justify-content: space-between;
       gap: 2px;
       padding: 2px;
       background-color: #fff;
       position: fixed;
       width: 100%;
       height: 80px;
       border-radius: 0%;
       bottom: 0;
       left: 0;
       transform: none;
   }

   .btn-proceed {
       background-color: #42DA5D;
       color: white;
       padding: 5px;
       width: 170px;
       border: none;
       border-radius: 10px;
       font-size: 16px;
       height: 60%;
       cursor: pointer;
       margin-right: 15px;
       margin-top: 15px;
       transition: background-color 0.3s ease, transform 0.3s ease;
   }

   .btn-proceed:hover {
       transform: scale(1.05);
   }

   .total-amount {
       text-align: left;
       font-size: 22px;
       margin-left: 10px;
       font-weight: 500;
       margin-top: 15px;
   }

   .total-amount .quantity-display {
       font-size: 14px;
       text-align: left;
   }

   .payment-logos {
       margin-top: 0;
       display: flex;
       justify-content: center;
       gap: 2px;
   }
}
    </style>
</head>

<body>
    <div class="main">
        <div class="header">
            <div class="logo">
                <img src="https://bingocircus.co.in/wp-content/uploads/2024/09/cropped-BC-Logo-PNG.png"
                    alt="Bingo Logo" loading="lazy" >
            </div>
            <div>
                <h1>Bingo Circus</h1>
                <p>India's Biggest Circus</p>
            </div>
        </div>

        <div class="form-container">


            <form id="ticketForm">
                <h4>Venue: KPHB, Kukatpally Housing Board Colony, Beside NEXUS MALL,<br> Opp. Malaysian Township, Kukatpally, Hyderabad</h4>
                <input id="location" type="hidden" name="location" value="Kukatpally_Hydrabad">


                <div class="row-container">
                    <div class="container">

                        <label for="show-date">Date</label>
                        <select id="show-date" name="show-date" required>
                            <option value="" disabled selected>Select show-date</option>
                        </select>
                        <span id="date-error" class="error"></span>



                        <label for="show-time">Showtime:</label>
                        <div class="time-options">
                            <button type="button" class="time-btn" onclick="selectTime('13:00')" id="btn-13:00">01:00
                                PM</button>
                            <button type="button" class="time-btn" onclick="selectTime('16:00')" id="btn-16:00">04:00
                                PM</button>
                            <button type="button" class="time-btn" onclick="selectTime('19:00')" id="btn-19:00">07:00
                                PM</button>
                        </div>

                        <select id="show-time" name="show-time" required hidden>
                            <option value="13:00">1:00 PM</option>
                            <option value="16:00">4:00 PM</option>
                            <option value="19:00">7:00 PM</option>
                        </select>
                        <span id="time-error" class="error"></span>

                        <label for="category">Category</label>
                        <button type="button" class="category-btn" onclick="selectPlan('400')">₹400</button>
                        <button type="button" class="category-btn" onclick="selectPlan('500')">₹500</button>

                        <select id="ticket-plan" name="ticket-plan" required hidden>
                            <option value="400">₹400</option>
                            <option value="500">₹500</option>
                        </select>
                        <span id="plan-error" class="error"></span>


                        <label for="quantity">Quantity</label>
                        <div class="quantity-container">
                            <button type="button" id="minus-btn">-</button>
                            <input class="quantity-input" type="number" id="quantity" name="quantity" min="1" max="100"
                                value="1" required readonly>
                            <button type="button" id="plus-btn">+</button>
                        </div>

                    </div>

                    <div class="container">

                        <label for="name">Full Name:</label>
                        <input type="text" id="name" name="name" placeholder="Enter Your Full Name" required>
                        <span id="name-error" class="error"></span>







                        <label for="email">Email Address</label>
                        <input type="email" id="email" name="email" placeholder="Enter Your Email Address" required>
                        <span id="email-error" class="error"></span>







                        <label for="phone">Phone Number</label>
                        <input type="tel" id="phone" name="phone" placeholder="Enter Your Phone Number" required>
                        <span id="phone-error" class="error"></span>






                        <p class="info-text">
                            Important: Your ticket will be sent to your email address, please double-check that you've
                            entered a correct and active email to ensure you receive your ticket without any issues.</p>


                    </div>
                </div>


                <div class="pay-container">
                    <input type="hidden" id="total-amount-input" name="total-amount">
                    <div class="total-amount">
                        ₹<span id="total-amount">0</span>
                        <div class="quantity-display">
                            <span id="quantity-display">1</span> Tickets
                        </div>
                    </div>
                    <button type="button" id="pay-btn" class="btn-proceed">Proceed</button>
                </div>



            </form>


            <div class="payment-logos">
                <img src="https://cdn.iconscout.com/icon/free/png-512/free-razorpay-logo-icon-download-in-svg-png-gif-file-formats--payment-gateway-brand-logos-icons-1399875.png?f=webp&w=512"
                    alt="Razorpay">
                <img src="https://cdn.iconscout.com/icon/free/png-256/free-phonepe-logo-icon-download-in-svg-png-gif-file-formats--payment-app-application-indian-companies-pack-logos-icons-2249157.png?f=webp&w=256"
                    alt="PhonePe">
                <img src="https://cdn.iconscout.com/icon/free/png-256/free-upi-logo-icon-download-in-svg-png-gif-file-formats--unified-payments-interface-payment-money-transfer-logos-icons-1747946.png?f=webp&w=256"
                    alt="UPI">
                <img src="https://cdn.iconscout.com/icon/free/png-256/free-google-pay-logo-icon-download-in-svg-png-gif-file-formats--gpay-technology-social-media-vol-3-pack-logos-icons-2944906.png?f=webp&w=256"
                    alt="GPay">
            </div>


        </div>
    </div>

    <script src="https://checkout.razorpay.com/v1/checkout.js"></script>
    <script>
const schedule = {
    Kukatpally_Hydrabad: {
        start: new Date('2024-12-15T00:00:00'), // Start time on 15 Dec 2024
        end: new Date('2025-01-15T23:59:59')    // End time on 15 Jan 2025
    }
};

        const timeSlots = [
            { time: "13:00", label: "1:00 PM" },
            { time: "16:00", label: "4:00 PM" },
            { time: "19:00", label: "7:00 PM" }
        ];
        function selectTime(time) {
            document.getElementById('show-time').value = time;
            document.querySelectorAll('.time-btn').forEach(btn => btn.classList.remove('active'));
            document.querySelector(`button[onclick="selectTime('${time}')"]`).classList.add('active');
        }

        function selectPlan(plan) {
            document.getElementById('ticket-plan').value = plan;
            document.querySelectorAll('.category-btn').forEach(btn => btn.classList.remove('active'));
            document.querySelector(`button[onclick="selectPlan('${plan}')"]`).classList.add('active');
            updateTotalAmount();
        }

        // Ensure the date dropdown is populated with available options
        function populateDateOptions() {
            const showDateSelect = document.getElementById('show-date');
            const location = document.getElementById('location').value;
            const today = new Date();
            showDateSelect.innerHTML = '<option value="" disabled selected>Select show-date</option>';

            if (location && schedule[location]) {
                let current = new Date(schedule[location].start);
                const end = new Date(schedule[location].end);
                let dateCount = 0;

                if (current < today) {
                    current = today;
                }

                while (current <= end && dateCount < 10) {
                    let option = document.createElement('option');
                    let dateString = current.toISOString().split('T')[0];
                    option.value = dateString;

                    let formattedDate = current.toLocaleDateString('en-US', {
                        year: 'numeric', month: 'short', day: 'numeric', weekday: 'short'
                    });
                    option.textContent = formattedDate;

                    showDateSelect.appendChild(option);
                    current.setDate(current.getDate() + 1);
                    dateCount++;
                }
            }
        }

        function disablePastShowTimes() {
            const selectedDate = document.getElementById('show-date').value;
            const today = new Date();
            const currentTime = today.getTime();
            
            // Disable all time buttons by default
            document.querySelectorAll('.time-btn').forEach(btn => btn.disabled = true);

            if (selectedDate) {
                const selectedDateObj = new Date(selectedDate);
                const isToday = selectedDateObj.toDateString() === today.toDateString();
                
                // Enable all time buttons for future dates
                if (!isToday) {
                    document.querySelectorAll('.time-btn').forEach(btn => btn.disabled = false);
                    return;
                }

                // For today's date, check each time slot
                timeSlots.forEach(slot => {
                    const slotTime = new Date(`${selectedDate}T${slot.time}`);
                    const timeDifference = slotTime.getTime() - currentTime;
                    
                    // Enable slot if it's more than 30 minutes in the future
                    const btn = document.getElementById(`btn-${slot.time}`);
                    if (btn) {
                        btn.disabled = timeDifference <= 30 * 60 * 1000;
                    }
                });
            }
        }

        document.getElementById('show-date').addEventListener('change', disablePastShowTimes);
        function updateTotalAmount() {
            const ticketPlan = document.getElementById('ticket-plan').value;
            const quantity = parseInt(document.getElementById('quantity').value) || 0;
            const totalAmountDisplay = document.getElementById('total-amount');
            const totalAmountInput = document.getElementById('total-amount-input');
            const quantityDisplay = document.getElementById('quantity-display');

            if (ticketPlan && quantity > 0) {
                const totalAmount = parseInt(ticketPlan) * quantity;
                totalAmountDisplay.textContent = totalAmount.toLocaleString('en-IN');
                totalAmountInput.value = totalAmount;
                quantityDisplay.textContent = quantity;
            } else {
                totalAmountDisplay.textContent = '0';
                totalAmountInput.value = '0';
                quantityDisplay.textContent = '0';
            }
        }


        window.onload = function () {
            populateDateOptions();
            
            const quantityInput = document.getElementById('quantity');
            const plusBtn = document.getElementById('plus-btn');
            const minusBtn = document.getElementById('minus-btn');
            const MAX_TICKETS = 200;

            function updateQuantity(newValue) {
                if (newValue >= 1 && newValue <= MAX_TICKETS) {
                    quantityInput.value = newValue;
                    updateTotalAmount();
                }
            }

            plusBtn.addEventListener('click', () => {
                const currentValue = parseInt(quantityInput.value) || 0;
                if (currentValue < MAX_TICKETS) {
                    updateQuantity(currentValue + 1);
                } else {
                    alert(`Maximum ${MAX_TICKETS} tickets allowed per booking.`);
                }
            });

            minusBtn.addEventListener('click', () => {
                const currentValue = parseInt(quantityInput.value) || 0;
                if (currentValue > 1) {
                    updateQuantity(currentValue - 1);
                }
            });

            // Prevent manual input of invalid quantities
            quantityInput.addEventListener('input', function() {
                let value = parseInt(this.value) || 0;
                if (value < 1) value = 1;
                if (value > MAX_TICKETS) value = MAX_TICKETS;
                updateQuantity(value);
            });

            // Update total when ticket plan changes
            document.getElementById('ticket-plan').addEventListener('change', updateTotalAmount);
        };
        function validateForm() {
            let isValid = true;
            const errors = {
                'show-date': 'Please select a show date.',
                'show-time': 'Please select a show time.',
                'ticket-plan': 'Please select a ticket plan.',
                'name': 'Please enter your name.',
                'email': 'Please enter a valid email address.',
                'phone': 'Please enter a valid phone number.'
            };

            // Clear all previous errors
            document.querySelectorAll('.error').forEach(error => error.textContent = '');

            // Validate required fields
            Object.keys(errors).forEach(fieldId => {
                const field = document.getElementById(fieldId);
                const errorElement = document.getElementById(`${fieldId}-error`);
                
                if (!field || !field.value.trim()) {
                    if (errorElement) {
                        errorElement.textContent = errors[fieldId];
                    }
                    isValid = false;
                }
            });

            // Validate email format
            const email = document.getElementById('email');
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (email && email.value.trim() && !emailRegex.test(email.value.trim())) {
                document.getElementById('email-error').textContent = 'Please enter a valid email address.';
                isValid = false;
            }

            // Validate phone number (10 digits)
            const phone = document.getElementById('phone');
            const phoneRegex = /^\d{10}$/;
            if (phone && phone.value.trim() && !phoneRegex.test(phone.value.trim())) {
                document.getElementById('phone-error').textContent = 'Please enter a valid 10-digit phone number.';
                isValid = false;
            }

            // Validate time and category selection
            if (!document.querySelector('.time-btn.active')) {
                document.getElementById('time-error').textContent = 'Please select a show time.';
                isValid = false;
            }

            if (!document.querySelector('.category-btn.active')) {
                document.getElementById('plan-error').textContent = 'Please select a ticket plan.';
                isValid = false;
            }

            return isValid;
        }

        // Add input validation listeners
        document.getElementById('email').addEventListener('input', function() {
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            const errorElement = document.getElementById('email-error');
            if (!emailRegex.test(this.value.trim())) {
                errorElement.textContent = 'Please enter a valid email address.';
            } else {
                errorElement.textContent = '';
            }
        });

        document.getElementById('phone').addEventListener('input', function() {
            const phoneRegex = /^\d{10}$/;
            const errorElement = document.getElementById('phone-error');
            if (!phoneRegex.test(this.value.trim())) {
                errorElement.textContent = 'Please enter a valid 10-digit phone number.';
            } else {
                errorElement.textContent = '';
            }
        });

        document.getElementById('pay-btn').addEventListener('click', function (e) {
            e.preventDefault();
            
            if (!validateForm()) {
                return;
            }

            const totalAmount = parseInt(document.getElementById('total-amount').textContent) * 100; // Convert to paise
            
            if (totalAmount <= 0) {
                alert('Please select tickets before proceeding to payment.');
                return;
            }

            const options = {
                "key": "rzp_live_Qg5QQIBVJbGsHs",
                "amount": totalAmount,
                "currency": "INR",
                "name": "Bingo Circus",
                "description": "Circus Ticket Booking",
                "image": "https://bingocircus.co.in/wp-content/uploads/2024/09/cropped-BC-Logo-PNG.png",
                "handler": function (response) {
                    handlePaymentSuccess(response);
                },
                "prefill": {
                    "name": document.getElementById('name').value,
                    "email": document.getElementById('email').value,
                    "contact": document.getElementById('phone').value
                },
                "theme": {
                    "color": "#3399cc"
                },
                "modal": {
                    "ondismiss": function() {
                        console.log('Payment modal closed');
                    }
                }
            };

            try {
                const rzp1 = new Razorpay(options);
                rzp1.open();
            } catch (error) {
                console.error('Error initializing Razorpay:', error);
                alert('There was an error initializing the payment gateway. Please try again later.');
            }
        });

        function handlePaymentSuccess(response) {
            if (!response || !response.razorpay_payment_id) {
                alert('Payment failed. Please try again.');
                return;
            }

            const formData = new FormData(document.getElementById('ticketForm'));
            formData.append('razorpay_payment_id', response.razorpay_payment_id);

            showLoader();

            fetch('save_booking.php', {
                method: 'POST',
                body: formData
            })
            .then(response => {
                if (!response.ok) {
                    throw new Error('Network response was not ok');
                }
                return response.text();
            })
            .then(data => {
                hideLoader();
                
                // Set a timeout to check for redirection
                const timeout = setTimeout(() => {
                    alert(`Payment successful but redirection failed. Payment ID: ${response.razorpay_payment_id}. Please contact support for assistance.`);
                }, 10000);

                // Redirect to ticket page
                window.location.href = `ticket.php?payment_id=${response.razorpay_payment_id}`;
                
                // Clear timeout if redirection happens
                clearTimeout(timeout);
            })
            .catch(error => {
                hideLoader();
                console.error('Error:', error);
                alert('An error occurred while processing your booking. Please contact support with your payment ID: ' + response.razorpay_payment_id);
            });
        }

        // Improve loader functions
        function showLoader() {
            const existingLoader = document.getElementById('loader');
            if (existingLoader) {
                return;
            }

            const loader = document.createElement('div');
            loader.id = 'loader';
            loader.style.position = 'fixed';
            loader.style.top = '0';
            loader.style.left = '0';
            loader.style.width = '100%';
            loader.style.height = '100%';
            loader.style.backgroundColor = 'rgba(0, 0, 0, 0.7)';
            loader.style.zIndex = '9999';
            loader.style.display = 'flex';
            loader.style.alignItems = 'center';
            loader.style.justifyContent = 'center';
            loader.innerHTML = `
                <div style="background: white; padding: 20px; border-radius: 10px; text-align: center;">
                    <div style="color: #333; font-size: 18px; margin-bottom: 10px;">Processing your booking...</div>
                    <div style="color: #666; font-size: 14px;">Please do not close this window</div>
                </div>
            `;
            document.body.appendChild(loader);
        }

        function hideLoader() {
            const loader = document.getElementById('loader');
            if (loader) {
                loader.remove();
            }
        }
    </script>
</body>

</html>
