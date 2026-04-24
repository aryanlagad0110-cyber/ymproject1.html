<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alpha Fitness Club</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body { font-family: Arial, sans-serif; }
        .hero { background: url('https://via.placeholder.com/1920x600?text=Gym+Background') no-repeat center center; background-size: cover; color: white; padding: 100px 0; }
        .plan { border: 1px solid #ddd; padding: 20px; margin: 10px; text-align: center; }
        .offer { background-color: #f8f9fa; padding: 10px; margin-top: 10px; }
        .registration-form { max-width: 600px; margin: 0 auto; }
    </style>
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <a class="navbar-brand" href="#">Alpha Fitness Club</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#plans">Membership Plans</a></li>
                    <li class="nav-item"><a class="nav-link" href="#register">Register</a></li>
                    <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <section id="home" class="hero">
        <div class="container text-center">
            <h1>Welcome to Alpha Fitness Club</h1>
            <p>Your ultimate destination for fitness and wellness. Join us to transform your body and mind.</p>
            <a href="#plans" class="btn btn-primary btn-lg">View Membership Plans</a>
        </div>
    </section>

    <section id="plans" class="py-5">
        <div class="container">
            <h2 class="text-center mb-4">Membership Plans</h2>
            <div class="row">
                <div class="col-md-4">
                    <div class="plan">
                        <h3>Basic Plan</h3>
                        <p>₹2600/month</p>
                        <ul class="list-unstyled">
                            <li>Access to gym equipment</li>
                            <li>Group classes</li>
                            <li>Locker room access</li>
                        </ul>
                        <div class="offer">
                            <strong>Offer:</strong> First month free!
                        </div>
                        <a href="#register" class="btn btn-success mt-3">Sign Up</a>
                    </div>
                </div>
                  <div class="col-md-4">
                    <div class="plan">
                        <h3>Premium Plan</h3>
                        <p>₹4400/month</p>
                        <ul class="list-unstyled">
                            <li>All Basic features</li>
                            <li>Personal trainer sessions (2x/week)</li>
                            <li>Nutrition consultation</li>
                        </ul>
                        <div class="offer">
                            <strong>Offer:</strong> 20% off annual subscription!
                        </div>
                        <a href="#register" class="btn btn-success mt-3">Sign Up</a>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="plan">
                        <h3>VIP Plan</h3>
                        <p>₹7100/month</p>
                        <ul class="list-unstyled">
                            <li>All Premium features</li>
                            <li>Unlimited personal training</li>
                            <li>Spa and sauna access</li>
                        </ul>
                        <div class="offer">
                            <strong>Offer:</strong> Free gym bag and water bottle!
                        </div>
                        <a href="#register" class="btn btn-success mt-3">Sign Up</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="register" class="py-5 bg-light">
        <div class="container">
            <h2 class="text-center mb-4">Register as a Member</h2>
            <form class="registration-form" id="registrationForm">
                <div class="mb-3">
                    <label for="name" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="name" name="name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email Address</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
                <div class="mb-3">
                    <label for="phone" class="form-label">Phone Number</label>
                    <input type="tel" class="form-control" id="phone" name="phone" required>
                </div>
                <div class="mb-3">
                    <label for="address" class="form-label">Residential Address</label>
                    <textarea class="form-control" id="address" name="address" rows="3" placeholder="Street, City, State, ZIP" required></textarea>
                </div>
                <div class="mb-3">
                    <label for="plan" class="form-label">Select Membership Plan</label>
                    <select class="form-select" id="plan" name="plan" required>
                        <option value="">Choose a plan</option>
                        <option value="Basic">Basic Plan - ₹2600/month (First month free!)</option>
                        <option value="Premium">Premium Plan - ₹4400/month (20% off annual!)</option>
                        <option value="VIP">VIP Plan - ₹7100/month (Free gym bag and water bottle!)</option>
                    </select>
                </div>
                <button type="submit" class="btn btn-primary">Register</button>
            </form>
            <div id="message" class="mt-3"></div>
        </div>
    </section>

    <section id="contact" class="py-5">
        <div class="container text-center">
            <h2>Contact Us</h2>
            <p>Address: 123 Fitness St, Pune, MAHARASHTRA 413801</p>
            <p>Phone: 7378479141</p>
            <p>Email: alphafitnessclub333@email.com</p>
        </div>
    </section>

    <footer class="bg-dark text-white text-center py-3">
        <p>&copy; 2023 Alpha Fitness Club. All rights reserved.</p>
    </footer>

    <script src="
(function(doc){
  var scriptElm = doc.scripts[doc.scripts.length - 1];
  var warn = ['[ionicons] Deprecated script, please remove: ' + scriptElm.outerHTML];

  warn.push('To improve performance it is recommended to set the differential scripts in the head as follows:')

  var parts = scriptElm.src.split('/');
  parts.pop();
  parts.push('ionicons');
  var url = parts.join('/');

  var scriptElm = doc.createElement('script');
  scriptElm.setAttribute('type', 'module');
  scriptElm.src = url + '/ionicons.esm.js';
  warn.push(scriptElm.outerHTML);
  scriptElm.setAttribute('data-stencil-namespace', 'ionicons');
  doc.head.appendChild(scriptElm);

  
  scriptElm = doc.createElement('script');
  scriptElm.setAttribute('nomodule', '');
  scriptElm.src = url + '/ionicons.js';
  warn.push(scriptElm.outerHTML);
  scriptElm.setAttribute('data-stencil-namespace', 'ionicons');
  doc.head.appendChild(scriptElm)
  
  console.warn(warn.join('\n'));

})(document);"></script>
 
</body>
</html>
