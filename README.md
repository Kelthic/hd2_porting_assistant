__Separated repository of HD2 Porting Assistant__

## Helldivers II Porting Assistant

_Written for Blender 4.2_

This tool designed to safely synchronize structural data between original mesh objects and new meshes with duplicated names for game export pipelines via HD2SDK.

It helps prevent common rigging and deformation issues caused by:

* extra vertex groups
* mismatched group order
* incorrect object pivots
* accidental data drift between originals and new meshes
* transfers object-level custom properties

Personally, when creating new armor, I always duplicate the names of the necessary parts, imitating the original names. That is, the conditional original is “Torso_Undergarment_Slim_lod0,” and my new mesh is “Torso_Undergarment_Slim_lod0.001.”

The add-on will automatically:
* remove non-original vertex groups
* reorder groups correctly
* restore the original pivot

#### Only mesh objects are supported.
#### The add-on does not rename or merge vertex groups.
#### Original objects are never modified during synchronization.
