---
title: Microsoft Intune での通信経費の管理
description: Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。
ms.openlocfilehash: b7b5eab316b0ad1f9e4cc25a42e7f36de7981ea5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072300"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Microsoft Intune での通信経費の管理

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。

次の Graph リソースを使用して、Intune での通信費を管理できます。

- [通信経費の管理パートナー](intune-tem-telecomexpensemanagementpartner.md)
