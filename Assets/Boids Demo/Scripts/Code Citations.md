# Code Citations

## License: unknown
https://github.com/miketon/SymLink/blob/8ca355c57f15cd202c9bcb2471f63fcb8ba749a7/Unity/Assets/Shared/__MtonFrameWork/ExternalDependency/FreeFromGithub/Boids/BoidBehaviour.cs

```
the vectors.
        var direction = separation + alignment + cohesion;
        var rotation = Quaternion.From
```


## License: unknown
https://github.com/miketon/SymLink/blob/8ca355c57f15cd202c9bcb2471f63fcb8ba749a7/Unity/Assets/Shared/__MtonFrameWork/ExternalDependency/FreeFromGithub/Boids/BoidBehaviour.cs

```
the vectors.
        var direction = separation + alignment + cohesion;
        var rotation = Quaternion.FromToRotation(Vector3.forward, direction.normalized);

        // Applys the rotation with interpolation.
        if (rotation != currentRotation)
        {
            var ip = Mathf.Exp(-controller.rotationCoeff
```


## License: unknown
https://github.com/miketon/SymLink/blob/8ca355c57f15cd202c9bcb2471f63fcb8ba749a7/Unity/Assets/Shared/__MtonFrameWork/ExternalDependency/FreeFromGithub/Boids/BoidBehaviour.cs

```
the vectors.
        var direction = separation + alignment + cohesion;
        var rotation = Quaternion.FromToRotation(Vector3.forward, direction.normalized);

        // Applys the rotation with interpolation.
        if (rotation != currentRotation)
        {
            var ip = Mathf.Exp(-controller.rotationCoeff * Time.deltaTime);
            transform.rotation = Quaternion.Slerp(rotation, currentRotation, ip);
        }

        // Moves forawrd.
        transform.position = currentPosition + transform.forward * (velocity * Time.deltaTime);
```

