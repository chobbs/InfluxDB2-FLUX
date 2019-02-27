# Perl Module to interact with the InfluxDBv2 API


## Not ready for production yet!

Influxdb2-perl module allows you to interact with the Version2 API of InfluxDB. The module is STILL
under heavy development. and does not have much. Only one API
endpoint is available today for <health>.


## INSTALLATION

To install this module, run the following commands:

	perl Makefile.PL
	make
	make test
	make install

## SYNOPSIS

Passing <host> and <port> is optional, defaulting to the Influxdb2-perl defaults. Returns
an instance of InfluxDB2::FLUX.

```
    use InfluxDB2::FLUX;

    my $influx = InfluxDB2::FLUX->new();

    my $server_health = $influx->health();
    print "$server_health_result\n";

```
