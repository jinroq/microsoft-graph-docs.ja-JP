---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2320b997ddc4bb9fb39ef528eecaca8a7c452426
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931033"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams デバイスの使用状況レポート

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。 21Vianet によって運営されて、Microsoft Graph 中国では、これらの Api はサポートされていません。

マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型                              | 説明                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。 |
