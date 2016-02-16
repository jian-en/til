# Get my ip address and username

Let's start with the quick one: to know your own username

```bash
> whoami
FuJian
```

There are two kinds of ip addresses: internal and external. To get the external address is a http request to a third-party service:

```bash
> curl ipecho.net/plain
```

To get the internal ip address there are some keywords like `ifconfig` but it takes me some time to locate the info so use a grep command:

```bash
> ifconfig | grep inet
```

[source](http://osxdaily.com/2010/11/21/find-ip-address-mac/)