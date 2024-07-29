# ATO-data
Keyboard and mouse events dataset collected in ATO project

The presented dataset was computed from the data collected in the supervised experiment during the periods November 2018 - July 2019 
and August 2019 - December 2019 and was composed of $17\,407$ records from $157$ unique users. 

The median time of data recording for a single user was 17 minutes. The number of records per user varied from 8 to 801, with the median equal to 86. 
Among all users, 55 ones with at least 100 records were selected.  

## Experiment

The data have been collected using three web browsers, i.e. Internet Explorer, Mozilla Firefox, and Google Chrome. The data collection process consisted of two phases: the registration phase and the login phase.

Each user was asked to enter a login and password during the registration phase. Logins were chosen from a list common to all subjects containing English words and several Polish and English phrases. The login and password text to be typed in by a user was displayed on the screen to prevent copying it but made it clear for the user which text is expected to be typed in. This way attempts to type in too simple literals such as one-character passwords or passwords replicating the same character many times were prevented. Moreover, errors made when retyping login and password prompted by the application had to be corrected by a user. The application recorded additional keyboard and potentially pointing device events in such cases.

Passwords were generated randomly as English words, numbers, and special characters. In addition, some letters in these words were replaced by numbers, special characters, or the respective uppercase letters to provide the ultimate passwords the users requested to type in. Hence, the data collection process reflected the frequent real-life requirement of using non-Latin characters in passwords.

Users were asked to enter the drawn login data several times during the login phase. In this step, the login data consisted of a login and password - drawn from those used during registration -and another login selected from a list of words not used during registration. The unknown login was a new text not seen by the user in the registration step. Notably, the attempts to type in the same login and password by different persons were recorded this way. Hence, for each user, both credentials of this user and additional data, i.e. randomly selected credentials of other users, were typed in. Consequently, the data beyond login and password, i.e. the data typically entered in web applications during the authentication process, were collected for every user. This approach provided a more extensive set of events than the keystroke events resulting from typing in one combination of a login and password.

The registration and login phases were performed on the same device. Additionally, the user was asked to repeat the login phase on another device of their choice. During the data collection, keyboard and pointing device events were captured by JavaScript code executed in the web browser (used by the person typing in the data) and transmitted to a server-side application as a stream of raw events.

## Publication
 
 <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 TRANSITIONAL//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">

<head>
<meta http-equiv="content-type" content="text/html; charset=utf-8" />
<link rel="stylesheet" href="htmlExportStyleSheet.css" />

</head>

<body>
<div class="content">
<dl>
<dt class="Key" id="GRZENDA2023120736">GRZENDA2023120736</dt>
<dd class="Pub">
	<span class="Title">Evaluation of machine learning methods for impostor detection in web applications</span><br />
	<span class="Author">M. Grzenda, S. Kaźmierczak, M. Luckner, G. Borowik, and J. Mańdziuk</span><br />
	<span class="Journal">Expert Systems with Applications</span>&nbsp;
	<span class="Volume">231</span>&nbsp;
	<span class="Pages">120736</span>&nbsp;
	(<span class="Date">2023</span>)<br />
	<span class="URL"><a href="https://www.sciencedirect.com/science/article/pii/S0957417423012381">https://www.sciencedirect.com/science/article/pii/S0957417423012381</a></span><br />
	<span class="URL"><a href="https://doi.org/10.1016/j.eswa.2023.120736">https://doi.org/10.1016/j.eswa.2023.120736</a></span><br />
	<div class="Abstract">Applying machine learning (ML) methods to multi-factor authentication is becoming increasingly popular. However, there is no comprehensive methodology to evaluate biometric systems based on machine learning in the literature. This paper proposes a general methodology for evaluation the ML-based systems for impostor recognition/detection using biometric traits. This includes creation of learning and testing sets with appropriate size balance (proportion) between these sets, selecting the number of instances coming from different users, evaluation of the influence of the impostors number on their detection rate, and the impact of the number of records representing user’s behavior. In addition, we propose how the real data (possibly affected by account takeover attempts) could be used to extend the enrollment data to support the impostor detection. The proposed approach was used for a systematic comparison of an extensive set of ML and statistical methods. For some of them, the false acceptance rate (FAR) close to zero and false rejection rate (FRR) smaller than 0.05 in a supervised experiment were accomplished, proving the merit of certain ML-based approaches. Moreover, using the method proposed in the paper, a classifier trained on experimental data achieved FAR below 0.05 on the real-world data collected at an actual financial web page.</div>
</dd>

</dl>
</div>
</body>
</html>

 
 ## Dataset
The dataset is given in data.csv file

### Structure 

  *A_KEY_TIME_MEAN*   - Mean difference between pressing and releasing time for alphanumerical keys	 
  
  *BOTH_DEV_C_COUNT*  - Percentage of situations when mouse click occurred with alphanumeric key event	 
  
  *BOTH_DEV_CC_COUNT* - Percentage of situations when mouse click occurred with combination key events	 
  
  *BOTH_DEV_M_COUNT*  - Percentage of situations when the mouse cursor moved with the alphanumeric key event	 
  
  *CLUSTERED_KEYS*    - At least one functional and alphanumeric key used at the same time	 
  
  *CLUSTERED_NR_KEYS* - Not a reasonable combination of keys used at the same time	 
  
  *CLUSTERED_R_KEYS*  - At least one functional key and no more than one alphanumeric key used at the same time	 
  
  *DELETE_KEY*    - Delete key used	 
  
  *DELETE_KEYS*   - Number of deletion events	 
  
  *GAP_D1* - GAP_D9	 Deciles of periods between key events	 
  
  *GAP_SD*    - Standard deviation of periods between key events	 
  
  *KEY_COUNT* - The number of pressed keys	 
  
  *KEY_GAP_TIME_D1* - KEY_GAP_TIME_D9	 Deciles of flight time	 
  
  *KEY_TIME*  - Dwell time	 
  
  *KEY_TIME_D1* - KEY_TIME_D9	 Deciles of the difference between key pressing and releasing time	 
  
  *KEY_TIME_MEAN* - Mean of difference between key pressing and releasing time	 
  
  *MANY_KEYS_BY_KEY_PRESSED*  - Ratio of multiple-key pressed events to all key events	 
  
  *MOUSE_CLICK_RATIO* - Ratio of mouse clicks to mouse movement events	 
  
  *MOUSE_COUNT*   - Mouse events number	 
  
  *MOUSE_DDIR_D1* - MOUSE_DDIR_D8	 Summaric distance covered by mouse in each of eight directions	 
  
  *MOUSE_DIR_D1* - MOUSE_DIR_D9	 Deciles of angle measure for segments traced by mouse	 
  
  *MOUSE_DIST_D1* - MOUSE_DIST_D9	 Deciles of distance covered by mouse movements	 
  
  *MOUSE_GAP_D1* - MOUSE_GAP_D9	 Deciles of time between mouse events	 
  
  *MOUSE_SPEED_D1* - MOUSE_SPEED_D9	Deciles of mouse speed	 
  
  *MULTIPLE_KEYS_DOWN*    - Number of pressed keys	 
  
  *MULTIPLE_KEYS_DOWN_D1* - MULTIPLE_KEYS_DOWN_D9	 Deciles of keys pressed at the same time	 
  
  *MULTIPLE_KEYS_UP*	- Number of released keys	 
  
  *MULTIPLE_KEYS_UP_D1* - MULTIPLE_KEYS_UP_D9	 Deciles of keys released at the same time	 
  
  *R_DELETE*  - The number of sequences using delete to remove the last character	 
  
  *R_DELETE_FREQ* - The frequency of sequences using delete to remove the last character	 
  
  *S_KEY_TIME_MEAN*   - Mean difference between pressing and releasing time for special keys	
