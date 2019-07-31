---
title: Microsoft Teams デバイスの使用状況レポート
description: 'Microsoft Teams デバイスの使用状況レポートを使用して、組織内の Microsoft Teams デバイスの使用状況に関する洞察を得ることができます。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0beada44b46afad1b8a51358f18259374a654f14
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966714"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams デバイスの使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams デバイスの使用状況レポートを使用して、組織内の Microsoft Teams デバイスの使用状況に関する洞察を得ることができます。 

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsdeviceusageuserdetail.md) | [Teamsdeviceの使い方 Userdetail](../resources/teamsdeviceusageuserdetail.md) | ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsdeviceusageusercounts.md) | [Teamsdevice使い方 User計数](../resources/teamsdeviceusageusercounts.md) | デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。 |
