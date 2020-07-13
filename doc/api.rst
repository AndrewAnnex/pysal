.. _api_ref:
=============
API Reference
=============

This is the class and function reference of pysal.

.. currentmodule:: pysal.lib


:mod:`pysal.lib`: PySAL Core 
=============================


Spatial Weights
---------------

.. autosummary::
   :toctree: generated/

   weights.W

Distance Weights
++++++++++++++++
.. autosummary::
   :toctree: generated/

   weights.DistanceBand
   weights.Kernel
   weights.KNN

Contiguity Weights
++++++++++++++++++

.. autosummary::
   :toctree: generated/

   weights.Queen
   weights.Rook
   weights.Voronoi
   weights.W

spint Weights
+++++++++++++

.. autosummary::
   :toctree: generated/

   weights.WSP
   weights.netW
   weights.mat2L
   weights.ODW
   weights.vecW


Weights Util Classes and Functions
++++++++++++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   weights.block_weights
   weights.lat2W
   weights.comb
   weights.order
   weights.higher_order
   weights.shimbel
   weights.remap_ids
   weights.full2W
   weights.full
   weights.WSP2W
   weights.get_ids
   weights.get_points_array_from_shapefile

Weights user Classes and Functions
++++++++++++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   weights.min_threshold_distance
   weights.lat2SW
   weights.w_local_cluster
   weights.higher_order_sp
   weights.hexLat2W
   weights.attach_islands
   weights.nonplanar_neighbors
   weights.fuzzy_contiguity
   weights.min_threshold_dist_from_shapefile
   weights.build_lattice_shapefile
   weights.spw_from_gal


Set Theoretic Weights
+++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   weights.w_union
   weights.w_intersection
   weights.w_difference
   weights.w_symmetric_difference
   weights.w_subset
   weights.w_clip


Spatial Lag
+++++++++++

.. autosummary::
   :toctree: generated/

   weights.lag_spatial
   weights.lag_categorical
          

cg: Computational Geometry
--------------------------

alpha_shapes
++++++++++++

.. autosummary::
   :toctree: generated/

   cg.alpha_shape
   cg.alpha_shape_auto

voronoi
+++++++

.. autosummary::
   :toctree: generated/

   cg.voronoi_frames


sphere
++++++

.. autosummary::
   :toctree: generated/

   cg.RADIUS_EARTH_KM
   cg.RADIUS_EARTH_MILES
   cg.arcdist
   cg.arcdist2linear
   cg.brute_knn
   cg.fast_knn
   cg.fast_threshold
   cg.linear2arcdist
   cg.toLngLat
   cg.toXYZ
   cg.lonlat
   cg.harcdist
   cg.geointerpolate
   cg.geogrid

shapes
++++++

.. autosummary::
   :toctree: generated/

   cg.Point
   cg.LineSegment
   cg.Line
   cg.Ray
   cg.Chain
   cg.Polygon
   cg.Rectangle
   cg.asShape

standalone
++++++++++

.. autosummary::
   :toctree: generated/

   cg.bbcommon
   cg.get_bounding_box
   cg.get_angle_between
   cg.is_collinear
   cg.get_segments_intersect
   cg.get_segment_point_intersect
   cg.get_polygon_point_intersect
   cg.get_rectangle_point_intersect
   cg.get_ray_segment_intersect
   cg.get_rectangle_rectangle_intersection
   cg.get_polygon_point_dist
   cg.get_points_dist
   cg.get_segment_point_dist
   cg.get_point_at_angle_and_dist
   cg.convex_hull
   cg.is_clockwise
   cg.point_touches_rectangle
   cg.get_shared_segments
   cg.distance_matrix


locators
++++++++

.. autosummary::
   :toctree: generated/

   cg.Grid
   cg.PointLocator
   cg.PolygonLocator


kdtree
++++++

.. autosummary::
   :toctree: generated/

   cg.KDTree


io
-- 

.. autosummary::
   :toctree: generated/

   io.open
   io.fileio.FileIO


examples
--------


.. autosummary::
   :toctree: generated/

   examples.available
   examples.explain
   examples.get_path

.. currentmodule:: pysal.explore

:mod:`pysal.explore`: Exploratory spatial data analysis
=======================================================

pysal.explore.esda: Spatial Autocorrelation Analysis
----------------------------------------------------

.. autosummary::
   :toctree: /generated

Gamma Statistic
+++++++++++++++

.. autosummary::
   :toctree: generated/

   esda.Gamma

.. _geary_api:

Geary Statistic
+++++++++++++++

.. autosummary::
   :toctree: generated/

   esda.Geary


.. _getis_api:

Getis-Ord Statistics
++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   esda.G
   esda.G_Local

.. _join_api:

Join Count Statistics
+++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   esda.Join_Counts

Moran Statistics
++++++++++++++++

.. autosummary::
   :toctree: generated/

   esda.Moran
   esda.Moran_BV
   esda.Moran_BV_matrix
   esda.Moran_Local
   esda.Moran_Local_BV
   esda.Moran_Rate
   esda.Moran_Local_Rate



pysal.explore.giddy: Geospatial Distribution Dynamics
-----------------------------------------------------


.. _markov_api:

Markov Methods
++++++++++++++

.. autosummary::
   :toctree: generated/

   giddy.markov.Markov
   giddy.markov.Spatial_Markov
   giddy.markov.LISA_Markov
   giddy.markov.FullRank_Markov
   giddy.markov.GeoRank_Markov
   giddy.markov.kullback
   giddy.markov.prais
   giddy.markov.homogeneity
   giddy.markov.sojourn_time
   giddy.ergodic.steady_state
   giddy.ergodic.fmpt
   giddy.ergodic.var_fmpt


.. _directional_api:

Directional LISA
++++++++++++++++

.. autosummary::
   :toctree: generated/

   giddy.directional.Rose


.. _mobility_api:

Economic Mobility Indices
+++++++++++++++++++++++++
.. autosummary::
   :toctree: generated/

    giddy.mobility.markov_mobility

.. _rank_api:

Exchange Mobility Methods
+++++++++++++++++++++++++
.. autosummary::
   :toctree: generated/

    giddy.rank.Theta
    giddy.rank.Tau
    giddy.rank.SpatialTau
    giddy.rank.Tau_Local
    giddy.rank.Tau_Local_Neighbor
    giddy.rank.Tau_Local_Neighborhood
    giddy.rank.Tau_Regional


pysal.explore.inequality: Spatial Inequality Analysis
-----------------------------------------------------

 .. _inequality_api:

Theil Inequality Measures
+++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    inequality.theil.Theil 
    inequality.theil.TheilD
    inequality.theil.TheilDSim


Gini Inequality Measures
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    inequality.gini.Gini_Spatial


pysal.explore.pointpats: Point Pattern Analysis
-----------------------------------------------

.. _pointpattern_api:

Point Pattern
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    pointpats.PointPattern

.. _pointprocess_api:

Point Processes
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    pointpats.PointProcess
    pointpats.PoissonPointProcess
    pointpats.PoissonClusterPointProcess

.. _centrgraphy_api:

Centrography
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    pointpats.mbr
    pointpats.hull
    pointpats.mean_center
    pointpats.weighted_mean_center
    pointpats.manhattan_median
    pointpats.std_distance
    pointpats.euclidean_median
    pointpats.ellipse
    pointpats.skyum
    pointpats.dtot
    pointpats._circle

.. _quadrat_api:

Quadrat Based Statistics
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    pointpats.RectangleM
    pointpats.HexagonM
    pointpats.QStatistic


.. _distance_api:

Distance Based Statistics
+++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    pointpats.DStatistic
    pointpats.G
    pointpats.F
    pointpats.J
    pointpats.K
    pointpats.L
    pointpats.Envelopes
    pointpats.Genv
    pointpats.Fenv
    pointpats.Jenv
    pointpats.Kenv
    pointpats.Lenv

.. _window_api:

Window functions
++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   pointpats.Window
   pointpats.as_window
   pointpats.poly_from_bbox
   pointpats.to_ccf


pysal.explore.segregation: Segregation Analysis
-----------------------------------------------

.. _segregation_api:

Aspatial Indices
+++++++++++++++++++++

.. autosummary::
   :toctree: generated/
   
      segregation.aspatial.Dissim 
      segregation.aspatial.GiniSeg
      segregation.aspatial.Entropy
      segregation.aspatial.Isolation
      segregation.aspatial.Exposure
      segregation.aspatial.Atkinson
      segregation.aspatial.CorrelationR
      segregation.aspatial.ConProf
      segregation.aspatial.ModifiedDissim
      segregation.aspatial.ModifiedGiniSeg
      segregation.aspatial.BiasCorrectedDissim
      segregation.aspatial.DensityCorrectedDissim

Spatial Indices
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
   
      segregation.spatial.SpatialProxProf
      segregation.spatial.SpatialDissim
      segregation.spatial.BoundarySpatialDissim
      segregation.spatial.PerimeterAreaRatioSpatialDissim
      segregation.spatial.DistanceDecayIsolation
      segregation.spatial.DistanceDecayExposure
      segregation.spatial.SpatialProximity
      segregation.spatial.AbsoluteClustering
      segregation.spatial.RelativeClustering
      segregation.spatial.Delta
      segregation.spatial.AbsoluteConcentration
      segregation.spatial.RelativeConcentration
      segregation.spatial.AbsoluteCentralization
      segregation.spatial.RelativeCentralization
	  
Multigroup Indices
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
   
      segregation.aspatial.MultiDissim
      segregation.aspatial.MultiGiniSeg
      segregation.aspatial.MultiNormalizedExposure
      segregation.aspatial.MultiInformationTheory
      segregation.aspatial.MultiRelativeDiversity
      segregation.aspatial.MultiSquaredCoefficientVariation
      segregation.aspatial.MultiDiversity
      segregation.aspatial.SimpsonsConcentration
      segregation.aspatial.SimpsonsInteraction
      segregation.aspatial.MultiDivergence
	  
Local Indices
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
   
      segregation.local.MultiLocationQuotient
      segregation.local.MultiLocalDiversity
      segregation.local.MultiLocalEntropy
      segregation.local.MultiLocalSimpsonInteraction
      segregation.local.MultiLocalSimpsonConcentration
      segregation.local.LocalRelativeCentralization
	  
Batch Compute Wrappers
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
   
	  segregation.compute_all.ComputeAllAspatialSegregation
	  segregation.compute_all.ComputeAllSpatialSegregation
	  segregation.compute_all.ComputeAllSegregation
	  
Inference Wrappers
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
   
	  segregation.inference.SingleValueTest
	  segregation.inference.TwoValueTest
	  
Decomposition
+++++++++++++++++++++
.. autosummary::
   :toctree: generated/
  
      segregation.decomposition.DecomposeSegregation

Network
+++++++++++++++++++++
.. autosummary::
 :toctree: generated/

      segregation.network.get_osm_network
      segregation.network.calc_access




pysal.explore.spaghetti: Spatial Analysis on Networks
-----------------------------------------------------


.. _spaghetti_api:


spaghetti.Network
+++++++++++++++++

.. autosummary::
   :toctree: generated/
    
    spaghetti.Network.extract_components
    spaghetti.Network.extractgraph
    spaghetti.Network.contiguityweights
    spaghetti.Network.distancebandweights
    spaghetti.Network.snapobservations
    spaghetti.Network.compute_distance_to_vertices
    spaghetti.Network.compute_snap_dist
    spaghetti.Network.count_per_link
    spaghetti.Network.simulate_observations
    spaghetti.Network.enum_links_vertex
    spaghetti.Network.full_distance_matrix
    spaghetti.Network.allneighbordistances
    spaghetti.Network.nearestneighbordistances
    spaghetti.Network.split_arcs
    spaghetti.Network.savenetwork
    spaghetti.Network.loadnetwork
    spaghetti.Network.NetworkF
    spaghetti.Network.NetworkG
    spaghetti.Network.NetworkK
    spaghetti.Network._evaluate_napts
    spaghetti.Network._extractnetwork
    spaghetti.Network._newpoint_coords
    spaghetti.Network._round_sig
    spaghetti.Network._snap_to_link
    spaghetti.Network._yield_napts
    spaghetti.Network._yieldneighbor


spaghetti.PointPattern
++++++++++++++++++++++

.. autosummary::
   :toctree: generated/
   
   spaghetti.PointPattern


spaghetti.SimulatedPointPattern
+++++++++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/
   
    spaghetti.SimulatedPointPattern


spaghetti
+++++++++

.. autosummary::
   :toctree: generated/
   
    spaghetti.element_as_gdf


.. currentmodule:: pysal.viz

:mod:`pysal.viz`: Geovisualization
==================================


pysal.viz.mapclassify: Choropleth map classification
----------------------------------------------------

.. _classifiers_api:

Classifiers
+++++++++++

.. autosummary::
   :toctree: generated/

   mapclassify.BoxPlot
   mapclassify.EqualInterval
   mapclassify.FisherJenks
   mapclassify.FisherJenksSampled
   mapclassify.HeadTailBreaks
   mapclassify.JenksCaspall
   mapclassify.JenksCaspallForced
   mapclassify.JenksCaspallSampled
   mapclassify.MaxP
   mapclassify.MaximumBreaks
   mapclassify.NaturalBreaks
   mapclassify.Quantiles
   mapclassify.Percentiles
   mapclassify.StdMean
   mapclassify.UserDefined

Utilities
+++++++++

.. autosummary::
   :toctree: generated/

   mapclassify.K_classifiers
   mapclassify.gadf

pysal.viz.splot: Lightweight visualization interface
----------------------------------------------------


Giddy
+++++

.. autosummary::
   :toctree: generated/

   splot.giddy.dynamic_lisa_heatmap
   splot.giddy.dynamic_lisa_rose
   splot.giddy.dynamic_lisa_vectors
   splot.giddy.dynamic_lisa_composite
   splot.giddy.dynamic_lisa_composite_explore


ESDA
++++

.. autosummary::
   :toctree: generated/

   splot.esda.moran_scatterplot
   splot.esda.plot_moran
   splot.esda.plot_moran_simulation
   splot.esda.plot_moran_bv
   splot.esda.plot_moran_bv_simulation
   splot.esda.lisa_cluster
   splot.esda.plot_local_autocorrelation
   splot.esda.moran_facet

Weights
+++++++

.. autosummary::
   :toctree: generated/

   splot.libpysal.plot_spatial_weights


mapping
+++++++

.. autosummary::
   :toctree: generated/

   splot.mapping.value_by_alpha_cmap
   splot.mapping.vba_choropleth
   splot.mapping.vba_legend
   splot.mapping.mapclassify_bin


 
.. currentmodule:: pysal.model
	
:mod:`pysal.model`: Linear models for spatial data analysis
===========================================================


pysal.model.spreg: Spatial Econometrics
---------------------------------------

These are the standard spatial regression models supported by the `spreg` package. Each of them contains a significant amount of detail in their docstring discussing how they're used, how they're fit, and how to interpret the results. 

.. autosummary::
   :toctree: generated/
    
   spreg.OLS
   spreg.ML_Lag
   spreg.ML_Error
   spreg.GM_Lag
   spreg.GM_Error
   spreg.GM_Error_Het
   spreg.GM_Error_Hom
   spreg.GM_Combo
   spreg.GM_Combo_Het
   spreg.GM_Combo_Hom
   spreg.GM_Endog_Error
   spreg.GM_Endog_Error_Het
   spreg.GM_Endog_Error_Hom
   spreg.TSLS
   spreg.ThreeSLS

Regimes Models
++++++++++++++

Regimes models are variants of spatial regression models which allow for structural instability in parameters. That means that these models allow different coefficient values in distinct subsets of the data. 

.. autosummary::
    :toctree: generated/

   spreg.OLS_Regimes
   spreg.ML_Lag_Regimes
   spreg.ML_Error_Regimes
   spreg.GM_Lag_Regimes
   spreg.GM_Error_Regimes
   spreg.GM_Error_Het_Regimes
   spreg.GM_Error_Hom_Regimes
   spreg.GM_Combo_Regimes
   spreg.GM_Combo_Hom_Regimes
   spreg.GM_Combo_Het_Regimes
   spreg.GM_Endog_Error_Regimes
   spreg.GM_Endog_Error_Hom_Regimes
   spreg.GM_Endog_Error_Het_Regimes

Seemingly-Unrelated Regressions
+++++++++++++++++++++++++++++++

Seeimingly-unrelated regression models are a generalization of linear regression. These models (and their spatial generalizations) allow for correlation in the residual terms between groups that use the same model. In spatial Seeimingly-Unrelated Regressions, the error terms across groups are allowed to exhibit a structured type of correlation: spatail correlation. 

.. autosummary::
   :toctree: generated/
    
   spreg.SUR
   spreg.SURerrorGM
   spreg.SURerrorML
   spreg.SURlagIV
   spreg.ThreeSLS


pysal.model.mgwr: Multiscale Geographically Weighted Regression
---------------------------------------------------------------

.. _mgwr_api:

GWR Model Estimation and Inference
++++++++++++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

   mgwr.gwr.GWR
   mgwr.gwr.GWRResults
   mgwr.gwr.GWRResultsLite


MGWR Estimation and Inference
+++++++++++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    mgwr.gwr.MGWR
    mgwr.gwr.MGWRResults


Kernel Specification
++++++++++++++++++++

.. autosummary::
   :toctree: generated/

    mgwr.kernels.Kernel
    mgwr.kernels.local_cdist

Bandwidth Selection
+++++++++++++++++++

.. autosummary::
   :toctree: generated/

   mgwr.sel_bw.Sel_BW


Visualization
+++++++++++++

.. autosummary::
   :toctree: generated/

   mgwr.utils.shift_colormap
   mgwr.utils.truncate_colormap
   mgwr.utils.compare_surfaces
