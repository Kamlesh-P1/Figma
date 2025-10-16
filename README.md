# Ex09 Event Registration Web Application
## Date:16-10-2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
section 1:
index.tsx
import React from "react";
import section1 from "./section-1.svg";

export const Box = (): JSX.Element => {
  return (
    <div className="w-[2500px] h-[650px]">
      <img
        className="fixed top-0 left-0 w-[2500px] h-[650px]"
        alt="Section"
        src={section1}
      />
    </div>
  );
};

tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame 1:
index.tsx
import React from "react";
import c15738c380F497FAb2BB9557Bfaa9B81 from "./8c15738c-380f-497f-ab2b-b9557bfaa9b8-1.png";

export const Frame = (): JSX.Element => {
  return (
    <div className="bg-white w-full min-w-[2500px] min-h-[5200px] relative">
      <img
        className="absolute top-0 left-0 w-[2500px] h-[5200px] aspect-[0.56] object-cover"
        alt="Sports Event Background"
        src={c15738c380F497FAb2BB9557Bfaa9B81}
      />

      <h1 className="absolute top-[863px] left-[272px] w-[1955px] [font-family:'Jua-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]">
        SPORTS EVENT 2025-2026
      </h1>

      <button
        className="absolute top-[3533px] left-[281px] w-[592px] h-[223px] bg-black cursor-pointer hover:opacity-90 transition-opacity"
        aria-label="Sign in to your account"
      >
        <span className="absolute top-[35px] left-0 w-[610px] [font-family:'Libre_Caslon_Text-Regular',Helvetica] font-normal text-[#fbf1f1] text-9xl text-center tracking-[0] leading-[normal]">
          Sign in
        </span>
      </button>

      <button
        className="absolute top-[3521px] left-[1400px] w-[750px] h-[250px] bg-[#130d0d] cursor-pointer hover:opacity-90 transition-opacity"
        aria-label="Register for a new account"
      >
        <span className="absolute top-[46px] left-[-300px] w-[1350px] [font-family:'Libre_Caslon_Text-Regular',Helvetica] font-normal text-[#fff7f7] text-9xl text-center tracking-[0] leading-[normal]">
          Register
        </span>
      </button>
    </div>
  );
};

tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame 2:
index.tsx
import React, { useState } from "react";
import abe9d5a706A64B1F812455B606B0A2331 from "./abe9d5a7-06a6-4b1f-8124-55b606b0a233-1.png";
import logo from "./logo.png";
import slice1 from "./slice-1.svg";

export const Frame = (): JSX.Element => {
  const [formData, setFormData] = useState({
    name: "",
    registerNumber: "",
    department: "",
    mobileNumber: "",
    email: "",
  });

  const handleInputChange = (field: string, value: string) => {
    setFormData((prev) => ({
      ...prev,
      [field]: value,
    }));
  };

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    console.log("Form submitted:", formData);
  };

  return (
    <div className="bg-white w-full min-w-[2500px] min-h-[5200px] relative">
      <img
        className="absolute w-[2500px] h-[660px] top-0 left-0"
        alt="Slice"
        src={slice1}
      />

      <div className="absolute top-0 left-0 w-[2500px] h-[660px] bg-[#d9d9d9]" />

      <img
        className="absolute top-[151px] left-14 w-[2387px] h-[359px] aspect-[6.65] object-cover"
        alt="Logo"
        src={logo}
      />

      <img
        className="absolute top-[660px] left-0 w-[2500px] h-[4450px] aspect-[1.03] object-cover"
        alt="Abeda a bf"
        src={abe9d5a706A64B1F812455B606B0A2331}
      />

      <form onSubmit={handleSubmit}>
        <div className="absolute top-[871px] left-[540px] w-[1320px] h-[310px] bg-black opacity-30" />

        <label
          htmlFor="name"
          className="absolute top-[941px] left-[460px] w-[1480px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]"
        >
          NAME
        </label>

        <input
          type="text"
          id="name"
          name="name"
          value={formData.name}
          onChange={(e) => handleInputChange("name", e.target.value)}
          className="absolute top-[871px] left-[540px] w-[1320px] h-[310px] bg-transparent z-10 [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal] px-4"
          aria-label="Name"
          required
        />

        <div className="absolute top-[1282px] left-[540px] w-[1320px] h-80 bg-[#110101] opacity-30" />

        <label
          htmlFor="registerNumber"
          className="absolute top-[1392px] left-[580px] w-[1280px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]"
        >
          REGISTER NUMBER
        </label>

        <input
          type="text"
          id="registerNumber"
          name="registerNumber"
          value={formData.registerNumber}
          onChange={(e) => handleInputChange("registerNumber", e.target.value)}
          className="absolute top-[1282px] left-[540px] w-[1320px] h-80 bg-transparent z-10 [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal] px-4"
          aria-label="Register Number"
          required
        />

        <div className="absolute top-[1793px] left-[540px] w-[1320px] h-[310px] bg-[#040000] opacity-30" />

        <label
          htmlFor="department"
          className="absolute top-[1903px] left-[610px] w-[1280px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]"
        >
          DEPARTMENT
        </label>

        <input
          type="text"
          id="department"
          name="department"
          value={formData.department}
          onChange={(e) => handleInputChange("department", e.target.value)}
          className="absolute top-[1793px] left-[540px] w-[1320px] h-[310px] bg-transparent z-10 [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal] px-4"
          aria-label="Department"
          required
        />

        <div className="absolute top-[3476px] left-[540px] w-[1280px] h-[330px] bg-[#160505] opacity-30" />

        <label
          htmlFor="mobileNumber"
          className="absolute top-[3523px] left-[540px] w-[1230px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]"
        >
          MOBILE NUMBER
        </label>

        <input
          type="tel"
          id="mobileNumber"
          name="mobileNumber"
          value={formData.mobileNumber}
          onChange={(e) => handleInputChange("mobileNumber", e.target.value)}
          className="absolute top-[3476px] left-[540px] w-[1280px] h-[330px] bg-transparent z-10 [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal] px-4"
          aria-label="Mobile Number"
          required
        />

        <div className="absolute top-[4024px] left-[515px] w-[1280px] h-[340px] bg-[#080000] opacity-30" />

        <label
          htmlFor="email"
          className="absolute top-[4076px] left-[490px] w-[1280px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-[#110202] text-9xl text-center tracking-[0] leading-[normal]"
        >
          EMAIL
        </label>

        <input
          type="email"
          id="email"
          name="email"
          value={formData.email}
          onChange={(e) => handleInputChange("email", e.target.value)}
          className="absolute top-[4024px] left-[515px] w-[1280px] h-[340px] bg-transparent z-10 [font-family:'Lilita_One-Regular',Helvetica] font-normal text-[#110202] text-9xl text-center tracking-[0] leading-[normal] px-4"
          aria-label="Email"
          required
        />

        <div className="absolute top-[4507px] left-[1573px] w-[870px] h-[250px] bg-[#990303] opacity-30" />

        <button
          type="submit"
          className="absolute top-[4507px] left-[1573px] w-[870px] h-[250px] bg-transparent z-10 cursor-pointer hover:opacity-80 transition-opacity"
          aria-label="Submit Form"
        >
          <span className="absolute top-[55px] left-[-10px] w-[890px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-[#4d521d] text-9xl text-center tracking-[0] leading-[normal]">
            SUBMIT
          </span>
        </button>
      </form>
    </div>
  );
};

tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame 3:
index.tsx
import React from "react";
import depositphotos69586581StockIllustrationProfessionalBadmintonPlayerColorfulHand1 from "./depositphotos-69586581-stock-illustration-professional-badminton-player-colorful-hand-1.png";
import logo2 from "./logo-2.png";

export const Frame = (): JSX.Element => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[2500px] min-h-[5200px] relative">
      <img
        className="absolute top-0 left-0 w-[2500px] h-[5121px] aspect-[0.67] object-cover"
        alt="Professional badminton player illustration"
        src={
          depositphotos69586581StockIllustrationProfessionalBadmintonPlayerColorfulHand1
        }
      />

      <img
        className="absolute top-[70px] left-[53px] w-[2393px] h-[360px] aspect-[6.65] object-cover"
        alt="Saveetha Engineering College Logo"
        src={logo2}
      />

      <div className="absolute top-[4219px] left-[53px] w-[1920px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]">
        CONTACT US :<br />
        <br />
        <br />
        NUMBER: 9876543210
        <br />
        EMAIL:ABC@gmail.com
      </div>

      <div className="absolute top-[760px] left-[172px] w-[1490px] [font-family:'Lilita_One-Regular',Helvetica] font-normal text-black text-9xl text-center tracking-[0] leading-[normal]">
        THANK YOU
      </div>
    </div>
  );
};

tailwind.config.js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer base {
  button,
  input,
  select,
  textarea {
    @apply appearance-none bg-transparent border-0 outline-none;
  }
}

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}
```

## OUTPUT:
<img width="1908" height="1135" alt="figma" src="https://github.com/user-attachments/assets/edb814a9-55bd-4810-8901-32da6fc84932" />


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
