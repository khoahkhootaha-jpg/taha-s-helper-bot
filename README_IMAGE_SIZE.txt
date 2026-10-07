Image generation dimensions are no longer hardcoded to 768x768.
The Pollinations native request omits width and height, and the OpenAI-compatible fallback omits size.
The selected image model/provider chooses its supported default dimensions. Provider-side maximums and model capabilities still apply.
