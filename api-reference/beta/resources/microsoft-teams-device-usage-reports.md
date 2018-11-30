---
title: Microsoft Teams デバイスの使用状況レポート
description: 'マイクロソフト チームのデバイスの使用状況レポートを使用すると、組織のマイクロソフト チームのデバイスの使用状況の洞察を取得できます。 '
ms.openlocfilehash: 22476c0891111d5f160e528477aab78ca5cc2e90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067263"
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
