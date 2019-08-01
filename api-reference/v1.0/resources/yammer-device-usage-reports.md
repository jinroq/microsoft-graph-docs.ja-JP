---
title: Yammer デバイス使用状況レポート
description: Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 209410e21cd9f96c87695409741e6a088a272601
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033265"
---
# <a name="yammer-device-usage-reports"></a>Yammer デバイス使用状況レポート

Yammer デバイス使用状況レポートでは、Yammer での取り組みにユーザーが利用しているデバイスに関する情報を取得できます。 一定期間中のデバイスの種類別ユーザーの数、およびユーザー別の詳細も確認することができます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Yammer デバイスの使用状況](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream      | ユーザー別の Yammer デバイス使用状況に関する詳細を取得します。 |
| [配布のユーザーの数を取得する](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream      | デバイスの種類別にユーザーの数を取得します。  |
| [ユーザーの数を取得する](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream      | デバイスの種類別に日次ユーザーの数を取得します。 |
