.. SM2ST documentation master file, created by
   sphinx-quickstart on Wed Feb 11 15:28:48 2026.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to SM2ST's documentation!
=================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:
   
   Normal_Resolution_SM2ST_masked_pearsonr_30o_rec
   Normal_Resolution_SM2ST_masked_pearsonr_30o_rec_STAGE
   Normal_Resolution_SM2ST_masked_pearsonr_30_rec_mask_03
   rectification41t2_SM2ST_test
   rectification31t2_SM2ST_test
   rectification31t2_STAGE_test
   SM2ST_Y7_T
   manual_rectification
   Multi_omics_Cluster
   Multi_omics_SpatialGlue_tutorial_smst
   super_Resolution_STMGraph_pyG1_30rex
.. image:: ../Images/fig1.png
   :width: 600

Introduction
=================

SM2ST: Spatial Mapping of Metabolomics onto Transcriptomics via Adversarial Regularized Autoencoders

Spatial transcriptomics, leveraging in situ sequencing or in situ hybridization, reveals the spatial distribution of gene expression at single-cell or sub-cellular resolution within tissue sections.  Concurrently, spatial metabolomics employs mass-spectrometry imaging (MSI), specifically MALDI-MS, to map metabolite distributions and provide molecular insight into metabolic activity.  Together, these techniques furnish complementary information on gene expression and metabolic dynamics for interrogating the tissue microenvironment.  However, the drift of MSI during the instrument’s long-term acquisition and the heterogeneity in its spatial chemical matrix coverage introduce noise that complicates cross-modal spatial alignment. Here we introduce an innovative multimodal registration framework that adopts hematoxylin-and-eosin (H&E) stained image as a bridging modality to compute adaptive affine transformations, aligning MSI with histological references and achieving landmark registration errors below 10 pixels. This process enables spatial transcriptomics and spatial metabolomics to be projected into a unified coordinate system. Building upon this, we propose a novel architectural framework that integrates generative adversarial networks (GANs) with autoencoders. This innovative approach enables effective denoising of metabolic ion signals and remapping onto spatial transcriptomic loci, thereby achieving point-to-point co-registration between the two modalities. The proposed method effectively addresses spatial heterogeneity across diverse data types, thereby enabling the development of a unified spatial multi-omics analytical framework. Furthermore, via a self-supervised super-resolution model termed STMGraph, we compensate for the limited sensitivity of high-mass molecules in conventional high-resolution MALDI-MS, effectively enhancing spatial metabolomic resolution.
