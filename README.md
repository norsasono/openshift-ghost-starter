# Inside This Package

- Nodejs v.6.9.5 (Recomended from Ghost)
- Ghost 0.11.11 (Latest stable version)

# How To?

1. Make a new Application using [Ghost 0.7.5 Quickstart](https://openshift.redhat.com/app/console/application_type/quickstart!240)
2. Use this repository as a source.
3. Done.

---

Don't worry, I actually use Node v.6.9.5 as the default cartridge because the default Node.js version from Openshift-Ghost-Quickstart is 0.10.** and no longger suppported for the recent Ghost version.

---

# Is it possible to be used to deploy Ghost v 1.0.-Beta?
Possiblly yes, but I haven’t tried. You know that Openshift provides you both Mysql (5.1 and 5.5) and Postgre (8.4 and 9.2), since Ghost doesn’t require the higher version of mysql, it is still possible. But remember, Ghost folks have dropped the support for PostgreSQL. Be wise.

Cheers .. 

