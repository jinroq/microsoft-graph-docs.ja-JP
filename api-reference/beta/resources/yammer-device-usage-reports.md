---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f5b24d6d235a8719f5f4b7df0389b5e5971dd8cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521867"
---
# <a name="yammer-device-usage-reports"></a>Yammer デバイス使用状況レポート

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | CSV の戻り値の型 | JSON の戻り値の型                         | 説明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | デバイスの種類別にユーザーの数を取得します。  |
| [ユーザーの数を取得する](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | デバイスの種類別に日次ユーザーの数を取得します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/yammer-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
