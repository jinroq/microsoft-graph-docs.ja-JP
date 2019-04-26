---
title: Microsoft Teams デバイスの使用状況レポート
description: 'microsoft teams デバイスの使用状況レポートを使用して、組織内の microsoft teams デバイスの使用状況に関する洞察を得ることができます。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 9521e458d72463f01fff116492bb240eaef35cf8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342241"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams デバイスの使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

microsoft teams デバイスの使用状況レポートを使用して、組織内の microsoft teams デバイスの使用状況に関する洞察を得ることができます。 

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsdeviceの使い方 userdetail](../resources/teamsdeviceusageuserdetail.md) | ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsdevice使い方 user計数](../resources/teamsdeviceusageusercounts.md) | デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。 |
