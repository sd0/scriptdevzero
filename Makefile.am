# Copyright (C) 2005-2011 MaNGOS <http://getmangos.com/>
#
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
## Process this file with automake to produce Makefile.in

## Sub-directories to parse
## NEED THE FIX SQL DIRECTORY....
##SUBDIRS = sql

BUILT_SOURCES = revision.h
CLEANFILES = revision.h
## CPP flags for includes, defines, etc.
AM_CPPFLAGS = $(MANGOS_INCLUDES) -I$(srcdir) -I$(srcdir)/../../../dep/include -I$(srcdir)/../../shared/ -I$(srcdir)/../../framework/ -I$(srcdir)/../../game/ -I$(srcdir)/include/ -I$(srcdir)/base/ -DSYSCONFDIR=\"$(sysconfdir)/\"

## Build MaNGOS script library as shared library.
# libmangosscript shared library will later be reused by world server daemon.
lib_LTLIBRARIES = libmangosscript.la
libmangosscript_la_SOURCES = \
ScriptMgr.cpp \
ScriptMgr.h \
config.h \
base/escort_ai.cpp \
base/escort_ai.h \
base/follower_ai.cpp \
base/follower_ai.h \
base/guard_ai.cpp \
base/guard_ai.h \
base/simple_ai.cpp \
base/simple_ai.h \
include/precompiled.cpp \
include/precompiled.h \
include/sc_creature.cpp \
include/sc_creature.h \
include/sc_gossip.h \
include/sc_grid_searchers.cpp \
include/sc_grid_searchers.h \
include/sc_instance.cpp \
include/sc_instance.h \
scripts/battlegrounds/battleground.cpp \
scripts/custom/custom.cpp \
scripts/custom/custom.h \
scripts/custom/custom_creatures.cpp \
scripts/custom/zero_creatures.cpp \
scripts/custom/zero_items.cpp \
scripts/eastern_kingdoms/alterac_mountains.cpp \
scripts/eastern_kingdoms/arathi_highlands.cpp \
scripts/eastern_kingdoms/blasted_lands.cpp \
scripts/eastern_kingdoms/burning_steppes.cpp \
scripts/eastern_kingdoms/dun_morogh.cpp \
scripts/eastern_kingdoms/eastern_plaguelands.cpp \
scripts/eastern_kingdoms/elwynn_forest.cpp \
scripts/eastern_kingdoms/hinterlands.cpp \
scripts/eastern_kingdoms/ironforge.cpp \
scripts/eastern_kingdoms/loch_modan.cpp \
scripts/eastern_kingdoms/redridge_mountains.cpp \
scripts/eastern_kingdoms/searing_gorge.cpp \
scripts/eastern_kingdoms/silverpine_forest.cpp \
scripts/eastern_kingdoms/stormwind_city.cpp \
scripts/eastern_kingdoms/stranglethorn_vale.cpp \
scripts/eastern_kingdoms/tirisfal_glades.cpp \
scripts/eastern_kingdoms/undercity.cpp \
scripts/eastern_kingdoms/western_plaguelands.cpp \
scripts/eastern_kingdoms/westfall.cpp \
scripts/eastern_kingdoms/wetlands.cpp \
scripts/eastern_kingdoms/blackrock_depths/blackrock_depths.cpp \
scripts/eastern_kingdoms/blackrock_depths/blackrock_depths.h \
scripts/eastern_kingdoms/blackrock_depths/boss_ambassador_flamelash.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_anubshiah.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_emperor_dagran_thaurissan.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_general_angerforge.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_gorosh_the_dervish.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_grizzle.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_high_interrogator_gerstahn.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_magmus.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_tomb_of_seven.cpp \
scripts/eastern_kingdoms/blackrock_depths/boss_coren_direbrew.cpp \
scripts/eastern_kingdoms/blackrock_depths/instance_blackrock_depths.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_drakkisath.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_gyth.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_halycon.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_highlord_omokk.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_mother_smolderweb.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_overlord_wyrmthalak.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_pyroguard_emberseer.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_quartermaster_zigris.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_rend_blackhand.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_shadow_hunter_voshgajin.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_the_beast.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_warmaster_voone.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_goraluk_anvilcrack.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_jed_runewatcher.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_mor_grayhoof.cpp \
scripts/eastern_kingdoms/blackrock_spire/boss_solakar_flamewreath.cpp \
scripts/eastern_kingdoms/blackrock_spire/brs_mob_trash.cpp \
scripts/eastern_kingdoms/blackrock_spire/instance_blackrock_spire.cpp \
scripts/eastern_kingdoms/blackrock_spire/blackrock_spire.h \
scripts/eastern_kingdoms/blackwing_lair/boss_broodlord_lashlayer.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_chromaggus.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_ebonroc.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_firemaw.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_flamegor.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_nefarian.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_razorgore.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_vaelastrasz.cpp \
scripts/eastern_kingdoms/blackwing_lair/boss_victor_nefarius.cpp \
scripts/eastern_kingdoms/blackwing_lair/instance_blackwing_lair.cpp \
scripts/eastern_kingdoms/blackwing_lair/blackwing_lair.h \
scripts/eastern_kingdoms/deadmines/deadmines.cpp \
scripts/eastern_kingdoms/deadmines/deadmines.h \
scripts/eastern_kingdoms/deadmines/instance_deadmines.cpp \
scripts/eastern_kingdoms/gnomeregan/boss_thermaplugg.cpp \
scripts/eastern_kingdoms/gnomeregan/gnomeregan.cpp \
scripts/eastern_kingdoms/gnomeregan/gnomeregan.h \
scripts/eastern_kingdoms/gnomeregan/instance_gnomeregan.cpp \
scripts/eastern_kingdoms/molten_core/boss_baron_geddon.cpp \
scripts/eastern_kingdoms/molten_core/boss_garr.cpp \
scripts/eastern_kingdoms/molten_core/boss_gehennas.cpp \
scripts/eastern_kingdoms/molten_core/boss_golemagg.cpp \
scripts/eastern_kingdoms/molten_core/boss_lucifron.cpp \
scripts/eastern_kingdoms/molten_core/boss_magmadar.cpp \
scripts/eastern_kingdoms/molten_core/boss_majordomo_executus.cpp \
scripts/eastern_kingdoms/molten_core/boss_ragnaros.cpp \
scripts/eastern_kingdoms/molten_core/boss_shazzrah.cpp \
scripts/eastern_kingdoms/molten_core/boss_sulfuron_harbinger.cpp \
scripts/eastern_kingdoms/molten_core/instance_molten_core.cpp \
scripts/eastern_kingdoms/molten_core/molten_core.cpp \
scripts/eastern_kingdoms/molten_core/molten_core.h \
scripts/eastern_kingdoms/naxxramas/boss_anubrekhan.cpp \
scripts/eastern_kingdoms/naxxramas/boss_faerlina.cpp \
scripts/eastern_kingdoms/naxxramas/boss_gluth.cpp \
scripts/eastern_kingdoms/naxxramas/boss_gothik.cpp \
scripts/eastern_kingdoms/naxxramas/boss_grobbulus.cpp \
scripts/eastern_kingdoms/naxxramas/boss_heigan.cpp \
scripts/eastern_kingdoms/naxxramas/boss_kelthuzad.cpp \
scripts/eastern_kingdoms/naxxramas/boss_four_horsemen.cpp \
scripts/eastern_kingdoms/naxxramas/boss_loatheb.cpp \
scripts/eastern_kingdoms/naxxramas/boss_maexxna.cpp \
scripts/eastern_kingdoms/naxxramas/boss_noth.cpp \
scripts/eastern_kingdoms/naxxramas/boss_patchwerk.cpp \
scripts/eastern_kingdoms/naxxramas/boss_razuvious.cpp \
scripts/eastern_kingdoms/naxxramas/boss_sapphiron.cpp \
scripts/eastern_kingdoms/naxxramas/boss_thaddius.cpp \
scripts/eastern_kingdoms/naxxramas/instance_naxxramas.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_arcanist_doan.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_azshir_the_sleepless.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_bloodmage_thalnos.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_herod.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_high_inquisitor_fairbanks.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_houndmaster_loksey.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_interrogator_vishas.cpp \
scripts/eastern_kingdoms/scarlet_monastery/boss_mograine_and_whitemane.cpp \
scripts/eastern_kingdoms/scarlet_monastery/instance_scarlet_monastery.cpp \
scripts/eastern_kingdoms/scarlet_monastery/scarlet_monastery.h \
scripts/eastern_kingdoms/scholomance/boss_darkmaster_gandling.cpp \
scripts/eastern_kingdoms/scholomance/boss_death_knight_darkreaver.cpp \
scripts/eastern_kingdoms/scholomance/boss_doctor_theolen_krastinov.cpp \
scripts/eastern_kingdoms/scholomance/boss_illucia_barov.cpp \
scripts/eastern_kingdoms/scholomance/boss_instructor_malicia.cpp \
scripts/eastern_kingdoms/scholomance/boss_jandice_barov.cpp \
scripts/eastern_kingdoms/scholomance/boss_kormok.cpp \
scripts/eastern_kingdoms/scholomance/boss_lord_alexei_barov.cpp \
scripts/eastern_kingdoms/scholomance/boss_lorekeeper_polkelt.cpp \
scripts/eastern_kingdoms/scholomance/boss_ras_frostwhisper.cpp \
scripts/eastern_kingdoms/scholomance/boss_the_ravenian.cpp \
scripts/eastern_kingdoms/scholomance/boss_vectus.cpp \
scripts/eastern_kingdoms/scholomance/instance_scholomance.cpp \
scripts/eastern_kingdoms/scholomance/scholomance.h \
scripts/eastern_kingdoms/shadowfang_keep/instance_shadowfang_keep.cpp \
scripts/eastern_kingdoms/shadowfang_keep/shadowfang_keep.cpp \
scripts/eastern_kingdoms/shadowfang_keep/shadowfang_keep.h \
scripts/eastern_kingdoms/stratholme/boss_baron_rivendare.cpp \
scripts/eastern_kingdoms/stratholme/boss_baroness_anastari.cpp \
scripts/eastern_kingdoms/stratholme/boss_cannon_master_willey.cpp \
scripts/eastern_kingdoms/stratholme/boss_dathrohan_balnazzar.cpp \
scripts/eastern_kingdoms/stratholme/boss_magistrate_barthilas.cpp \
scripts/eastern_kingdoms/stratholme/boss_maleki_the_pallid.cpp \
scripts/eastern_kingdoms/stratholme/boss_nerubenkan.cpp \
scripts/eastern_kingdoms/stratholme/boss_postmaster_malown.cpp \
scripts/eastern_kingdoms/stratholme/boss_ramstein_the_gorger.cpp \
scripts/eastern_kingdoms/stratholme/boss_timmy_the_cruel.cpp \
scripts/eastern_kingdoms/stratholme/instance_stratholme.cpp \
scripts/eastern_kingdoms/stratholme/stratholme.cpp \
scripts/eastern_kingdoms/stratholme/stratholme.h \
scripts/eastern_kingdoms/sunken_temple/instance_sunken_temple.cpp \
scripts/eastern_kingdoms/sunken_temple/sunken_temple.cpp \
scripts/eastern_kingdoms/sunken_temple/sunken_temple.h \
scripts/eastern_kingdoms/uldaman/boss_ironaya.cpp \
scripts/eastern_kingdoms/uldaman/uldaman.cpp \
scripts/eastern_kingdoms/zulgurub/boss_arlokk.cpp \
scripts/eastern_kingdoms/zulgurub/boss_gahzranka.cpp \
scripts/eastern_kingdoms/zulgurub/boss_grilek.cpp \
scripts/eastern_kingdoms/zulgurub/boss_hakkar.cpp \
scripts/eastern_kingdoms/zulgurub/boss_hazzarah.cpp \
scripts/eastern_kingdoms/zulgurub/boss_jeklik.cpp \
scripts/eastern_kingdoms/zulgurub/boss_jindo.cpp \
scripts/eastern_kingdoms/zulgurub/boss_mandokir.cpp \
scripts/eastern_kingdoms/zulgurub/boss_marli.cpp \
scripts/eastern_kingdoms/zulgurub/boss_renataki.cpp \
scripts/eastern_kingdoms/zulgurub/boss_thekal.cpp \
scripts/eastern_kingdoms/zulgurub/boss_venoxis.cpp \
scripts/eastern_kingdoms/zulgurub/boss_wushoolay.cpp \
scripts/eastern_kingdoms/zulgurub/instance_zulgurub.cpp \
scripts/eastern_kingdoms/zulgurub/zulgurub.h \
scripts/kalimdor/ashenvale.cpp \
scripts/kalimdor/azshara.cpp \
scripts/kalimdor/boss_azuregos.cpp \
scripts/kalimdor/darkshore.cpp \
scripts/kalimdor/desolace.cpp \
scripts/kalimdor/dustwallow_marsh.cpp \
scripts/kalimdor/felwood.cpp \
scripts/kalimdor/feralas.cpp \
scripts/kalimdor/moonglade.cpp \
scripts/kalimdor/mulgore.cpp \
scripts/kalimdor/orgrimmar.cpp \
scripts/kalimdor/silithus.cpp \
scripts/kalimdor/stonetalon_mountains.cpp \
scripts/kalimdor/tanaris.cpp \
scripts/kalimdor/teldrassil.cpp \
scripts/kalimdor/the_barrens.cpp \
scripts/kalimdor/thousand_needles.cpp \
scripts/kalimdor/thunder_bluff.cpp \
scripts/kalimdor/ungoro_crater.cpp \
scripts/kalimdor/winterspring.cpp \
scripts/kalimdor/blackfathom_deeps/blackfathom_deeps.h \
scripts/kalimdor/blackfathom_deeps/instance_blackfathom_deeps.cpp \
scripts/kalimdor/maraudon/boss_celebras_the_cursed.cpp \
scripts/kalimdor/maraudon/boss_landslide.cpp \
scripts/kalimdor/maraudon/boss_noxxion.cpp \
scripts/kalimdor/maraudon/boss_princess_theradras.cpp \
scripts/kalimdor/onyxias_lair/boss_onyxia.cpp \
scripts/kalimdor/razorfen_downs/boss_amnennar_the_coldbringer.cpp \
scripts/kalimdor/razorfen_downs/razorfen_downs.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_ayamiss.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_buru.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_kurinnaxx.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_moam.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_ossirian.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/boss_rajaxx.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/instance_ruins_of_ahnqiraj.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/ruins_of_ahnqiraj.cpp \
scripts/kalimdor/ruins_of_ahnqiraj/ruins_of_ahnqiraj.h \
scripts/kalimdor/temple_of_ahnqiraj/boss_bug_trio.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_cthun.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_fankriss.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_huhuran.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_ouro.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_sartura.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_skeram.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_twinemperors.cpp \
scripts/kalimdor/temple_of_ahnqiraj/boss_viscidus.cpp \
scripts/kalimdor/temple_of_ahnqiraj/instance_temple_of_ahnqiraj.cpp \
scripts/kalimdor/temple_of_ahnqiraj/mob_anubisath_sentinel.cpp \
scripts/kalimdor/temple_of_ahnqiraj/temple_of_ahnqiraj.h \
scripts/kalimdor/wailing_caverns/def_wailing_caverns.h \
scripts/kalimdor/wailing_caverns/instance_wailing_caverns.cpp \
scripts/kalimdor/wailing_caverns/wailing_caverns.cpp \
scripts/kalimdor/zulfarrak/zulfarrak.h \
scripts/kalimdor/zulfarrak/zulfarrak.cpp \
scripts/kalimdor/zulfarrak/boss_zumrah.cpp \
scripts/kalimdor/zulfarrak/instance_zulfarrak.cpp \
scripts/world/areatrigger_scripts.cpp \
scripts/world/boss_emeriss.cpp \
scripts/world/boss_lord_kazzak.cpp \
scripts/world/boss_lethon.cpp \
scripts/world/boss_taerar.cpp \
scripts/world/boss_ysondre.cpp \
scripts/world/go_scripts.cpp \
scripts/world/guards.cpp \
scripts/world/item_scripts.cpp \
scripts/world/mob_generic_creature.cpp \
scripts/world/npc_professions.cpp \
scripts/world/npcs_special.cpp \
system/ScriptLoader.cpp \
system/ScriptLoader.h \
system/system.cpp \
system/system.h \
revision.h


## magic to include revision data in SD2 version string
revision.h: FORCE
	$(top_builddir)/src/tools/genrevision/genrevision $(srcdir)

FORCE:

## libtool settings
# API versioning
# Link against dependencies
# How to increase version info:
# - only bug fixes implemented:
# bump the version to LTMANGOS_CURRENT:LTMANGOS_REVISION+1:LTMANGOS_AGE
# - augmented the interface:
# bump the version to LTMANGOS_CURRENT+1:0:LTMANGOS_AGE+1
# - broken old interface:
# bump the version to LTMANGOS_CURRENT+1:0:0
LTMANGOS_CURRENT = 0
LTMANGOS_REVISION = 0
LTMANGOS_AGE = 0
libmangosscript_la_LIBFLAGS = -version-info $(LTMANGOS_CURRENT):$(LTMANGOS_REVISION):$(LTMANGOS_AGE)

## Additional files to include when running 'make dist'
# Scripts defaults.
EXTRA_DIST = \
	Scripts/sc_default.cpp \
	Scripts/sc_defines.cpp \
	Scripts/sc_defines.h \
	scriptdevzero.conf.dist

## Additional files to install
sysconf_DATA = \
	scriptdevzero.conf.dist

install-data-hook:
	@list='$(sysconf_DATA)'; for p in $$list; do \
      dest=`echo $$p | sed -e s/.dist//`; \
	  if test -f $(DESTDIR)$(sysconfdir)/$$dest; then \
        echo "$@ will not overwrite existing $(DESTDIR)$(sysconfdir)/$$dest"; \
      else \
	    echo " $(INSTALL_DATA) $$p $(DESTDIR)$(sysconfdir)/$$dest"; \
	    $(INSTALL_DATA) $$p $(DESTDIR)$(sysconfdir)/$$dest; \
	  fi; \
	done

clean-local:
	rm -f $(sysconf_DATA)
