# Metex

Learning OTP and GenServer. Small application to test a GenServer application.
The GenServer process uses an API service to read temperatures of cities around the world.

Taken from the book _The little Elixir and OTP guidebook_ from _Benjamin Tan Wei Hao_.

## Installation

- Run mix deps.get to install dependencies
- get an API key from https://openweathermap.org
- write the api key at the top of lib/worker.ex (@api_key)

## Usage

- Start iex -S mix
- Start the process:
  `Metex.Worker.start_link`
- Call for temperatures around the world: `Metex.Worker.get_temperature("Quebec")`
