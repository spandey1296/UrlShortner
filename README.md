# UrlShortner



<ul>
<li>
Given a URL, Our service should generate a shortner and unique alias of it. This is called a short link.
This link should be short enough to be easily copied and pasted into applications.
</li>
<li>

when users access a short link, our application should redirect them to the original link.

</li>
<li>
The generated link should have a standard expiration time. Optionally users should be able to define the link expiration time.


</li>

</ul>

# RESTAPI:

<ul>
  <li>
createURl(original_url, expire_date=None)::POST
Parameters:
original_url(String):URL to be shortened.
expire_date(String):Optional expiry date for shortened url

  </li>
  <li>

2. deleteURL(short_url)::DELETE
Parameters:
short_url(String):short url to be deleted.
  </li>
  <li>

3. redirect(short_url):: GET
Parameters:
short_url(String): short URL to be redirected to the original link.
  </li>
</ul>

  
# Database Design:

<p> URL      DataTypes

original_url  club
short_url     varchar
create_at     Timestamp
expires_at    Timestamp
</p>



# Developed By: <P> Shivant Kumar Pandey</p>









