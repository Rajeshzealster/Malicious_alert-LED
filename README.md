# Malicious_alert-LED
An application to alert malicious activities with LED blink

## Project Description

The Malicious Alert-LED project is a security monitoring system that detects malicious activities on your application and signals them by blinking an LED. The entire application is deployed on Raspberry Pi devices using a K3s cluster. When any suspicious activity is detected on the application page, an LED attached to one of the Raspberry Pi devices in the cluster will blink as an alert.

This project leverages the use of TOSCA to model the entire application and xOpera to dynamically deploy the application using simple adhoc commands on remote Raspberry Pi devices. xOpera utilizes Ansible playbooks to manage the necessary configurations for the application and establishes SSH connections to the remote devices.

## Features

- Real-time monitoring of application activities.
- Immediate alerting through LED blinking.
- Scalable deployment on Raspberry Pi clusters using K3s.
- TOSCA-based modeling for application components.
- Dynamic deployment and configuration management using xOpera and Ansible.

## Installation

To deploy and use this project, follow these steps:

1. **Prerequisites**: Ensure you have the following prerequisites installed:
   - [K3s](https://k3s.io/) cluster set up on Raspberry Pi devices.
   - [TOSCA](http://www.oasis-open.org/committees/tc_home.php?wg_abbrev=tosca) for modeling the application.
   - [xOpera](https://xopera-docs.readthedocs.io/en/latest/) for dynamic deployment.

2. **Clone the Repository**: Clone this repository to your local machine.

3. **Configuration**: Configure the project as per your requirements by modifying the TOSCA templates and Ansible playbooks.

4. **Deployment**: Use xOpera to deploy the application onto your Raspberry Pi cluster. For more detailed list of commands offered by xOpera, please refer [xOpera CLI](https://xlab-si.github.io/xopera-docs/02-cli.html)

5. **Monitoring**: Once deployed, the system will continuously monitor your application for malicious activities.

## Usage

- Start the monitoring process by executing the deployment command.
- Monitor the LED on the Raspberry Pi cluster for alerts.
- Refer to the logs for detailed information about detected malicious activities.

## Contributing

If you would like to contribute to this project, please open an issue or submit a pull request. We welcome your contributions.


## Contact

For questions or feedback, feel free to contact the project maintainer:
- Rajesh Thalla - <rajeshzealster@gmail.com>

