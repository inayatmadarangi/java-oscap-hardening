Role Name
=========

Secure Configuration of Java Runtime Environment

Refer to
https://static.open-scap.org/ssg-guides/ssg-jre-guide-index.html

Requirements
------------
Java is a general-purpose computer programming language. It is intended to let application developers "write once, run anywhere." Java applications are typically compiled to bytecode that can run on any Java virtual machine (JVM) regardless of computer architecture. As such, the Java runtime environment (JRE) is required to be installed so that Java applications can run. This section provides settings for configuring Java policies to meet compliance settings for Java running on Red Hat Enterprise Linux systems.

Refer to
https://docs.oracle.com/javase/6/docs/technotes/guides/deployment/deployment-guide/properties.html
for a list of currently supported Java version 6 settings.
Refer to
https://docs.oracle.com/javase/7/docs/technotes/guides/jweb/jcp/properties.html
for a list of currently supported Java version 7 settings.
Refer to
https://docs.oracle.com/javase/8/docs/technotes/guides/deploy/properties.html
for a list of currently supported Java version 8 settings.



Role Variables
--------------
- Severity Execution
high_severity
medium_severity
- Complexity Execution
low_complexity
- Distruption Execution
low_disruption
- Java Control Specific Execution
java_jre_accepted_sites_properties
java_jre_blacklist_check
java_jre_blacklist_check_locked
java_jre_clean_previous_version
java_jre_deployment_config_exists
java_jre_deployment_config_mandatory
java_jre_deployment_config_properties
java_jre_deployment_properties_exists
java_jre_disable_untrusted_sources
java_jre_disable_untrusted_sources_locked
java_jre_enable_jws
java_jre_enable_jws_locked
java_jre_insecure_prompt
java_jre_insecure_prompt_locked
java_jre_lock_untrusted_sources
java_jre_lock_untrusted_sources_locked
java_jre_security_revocation_check
java_jre_security_revocation_check_locked
java_jre_unsigned_applications
java_jre_unsigned_applications_locked
java_jre_validation_crl
java_jre_validation_crl_locked
java_jre_validation_ocsp
java_jre_validation_ocsp_locked

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }
    ---
    - name: Java Hardening OSCAP
      user: inayat
      hosts: localhost
      become: true
  

      roles:
        - java-oscap-hardening

License
-------

BSD

Author Information
------------------

