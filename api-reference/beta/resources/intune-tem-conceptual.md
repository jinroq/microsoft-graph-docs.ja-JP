---
title: Microsoft Intune での通信経費管理-Microsoft Graph API
description: テナント組織の通信経費管理に関連した Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 9856f01337d7ed6af6fc6df6c2e3e118b762ca0a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938619"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Microsoft Intune での通信経費の管理

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。

次の Graph リソースを使用して、Intune での通信費を管理できます。

- [通信経費の管理パートナー](intune-tem-telecomexpensemanagementpartner.md)
