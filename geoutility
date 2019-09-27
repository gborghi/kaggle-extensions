def getdistance(lat1,long1, lat2, long2):
    from math import sin, cos, sqrt, atan2, radians

    # approximate radius of earth in km
    R = 6373.0

    lat1r = radians(lat1)
    lon1r = radians(long1)
    lat2r = radians(lat2)
    lon2r = radians(long2)

    dlon = lon2r - lon1r
    dlat = lat2r - lat1r

    a = sin(dlat / 2)**2 + cos(lat1r) * cos(lat2r) * sin(dlon / 2)**2
    c = 2 * atan2(sqrt(a), sqrt(1 - a))

    distance = R * c
    return distance
