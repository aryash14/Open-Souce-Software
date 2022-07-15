# Check 1:

<img width="863" alt="image" src="https://user-images.githubusercontent.com/71746459/179249715-04e0b287-3f5e-423c-bb85-6b7b62352282.png">

# Check 2:

Find the Nightly and Experimental sections and look at some of the submissions. How can you see what tests were run for a particular submission?
- Number of Not run + Fail + Pass would be the number of tests ran.
Find a submission with errors. Can you see what the error condition was? How does this help you debug the failure?
Yes the error is with a  file not being found in our case this file is openssl/opensslconf.h and the error is fatal error: openssl/opensslconf.h: No such file or directory
And when the code hits #include <openssl/opensslconf.h> it terminates the compilation
Find a system that is close to your specific configuration in the Nightly, Nightly Expected or one of the Masters sections. How clean is the dashboard? Are there any errors that you need to be concerned with?
Dashbord shows how many tests failed and how any passes. We can also see errors and warning there are.

No erros with my submission. Which was consistent with programs that had the same structure as mine.

<img width="1415" alt="image" src="https://user-images.githubusercontent.com/71746459/179254177-f1f51aea-d066-4e00-a0f4-f8e24b714820.png">

<img width="1440" alt="image" src="https://user-images.githubusercontent.com/71746459/179254222-38116d94-7b65-406b-993d-ad7e9880baa1.png">

# Check 3:

Information provided for the failure is below. Which told me the test failing and why it is failing.
CMake Error at /Users/aryash/Documents/GitHub/cmake/Tests/CMakeCopyright.cmake:9 (message):
  Copyright.txt contains

   Copyright 2000-2020 Kitware, Inc. and Contributors

  but the current version year is 2022.

Instead of having to go into LastTest.log to see what the error message was -VV simply displayed it on the terminal when I ran the tests.

Test submission with errors: 

<img width="805" alt="image" src="https://user-images.githubusercontent.com/71746459/179256475-c5bead28-3662-492e-8b3f-f9e9b2cd740e.png">

After changing LESS to GREATER in CMakeCopyRight.cmake this it the output:

<img width="588" alt="image" src="https://user-images.githubusercontent.com/71746459/179258031-1707539d-ccc1-4196-90fb-581d7867568c.png">

# Check 4:

