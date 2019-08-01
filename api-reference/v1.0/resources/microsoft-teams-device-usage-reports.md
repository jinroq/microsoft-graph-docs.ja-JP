---
title: Microsoft Teams デバイスの使用状況レポート
description: Microsoft Teams デバイスの使用状況レポートを使用して、組織内の Microsoft Teams デバイスの使用状況に関する情報を取得します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: ebac2c81b613b967ca6c559a586c349e59d0c552
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036079"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams デバイスの使用状況レポート

Microsoft Teams デバイスの使用状況レポートを使用して、組織内の Microsoft Teams デバイスの使用状況に関する情報を取得します。

## <a name="methods"></a>メソッド

| メソッド                                   | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getteamsdeviceusageuserdetail.md) | Stream      | ユーザーごとに、Microsoft Teams デバイスの使用状況の詳細を取得します。 |
| [ユーザーの数を取得する](../api/reportroot-getteamsdeviceusageusercounts.md) | Stream      | デバイスの種類ごとに、日次ユニーク ユーザーの数を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | ストリーム      | デバイスの種類ごとに、選択した期間のユニーク ユーザーの数を取得します。 |
