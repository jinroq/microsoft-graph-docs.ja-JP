---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d19df5132a67ac5862535a329eadbdff7044798c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576641"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams デバイスの使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
