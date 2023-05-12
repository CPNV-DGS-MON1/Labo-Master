# Load testing

* [x] Add htop to your Linux vm

```
apt-get install htop
```

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption><p>Htop view</p></figcaption></figure>

* [x] Add stress to your Linux vm and try to stress your cpu

```
apt-get install stress
```

<!---->

* [Stress documentation](https://www.golinuxcloud.com/stress-command-in-linux/)

<!---->

* [x] In two ssh windows, stress your vm and observe the CPU load with htop

```
stress -c N OR stress --cpu N
```

![image-20230512135439033](assets/image-20230512135439033.png)

##### htop - Sans stress

![image-20230512135141489](assets/image-20230512135141489.png)



<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Htop view with load on CPU</p></figcaption></figure>

##### htop - Avec stress

![image-20230512135318997](assets/image-20230512135318997.png)

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption><p>Htop view with load on CPU</p></figcaption></figure>

* [x] Observer the CPU peak on NewRelic

![image-20230512135353538](assets/image-20230512135353538.png)

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>CPU Peak on New Relic</p></figcaption></figure>

![image-20230512135519926](assets/image-20230512135519926.png)
