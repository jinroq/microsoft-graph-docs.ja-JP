---
title: Microsoft Intune での通信経費の管理
description: Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: b2d581c6c10a1782a1b75be37f7b040f3c9dbd3b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036814"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Microsoft Intune での通信経費の管理

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。

Intune と統合している、Saaswedo 通信経費管理サービスを使用すると、会社所有のデバイスでのデータの使用とローミングを制限することができます。 このサービスを使用すると、使用制限を設定および適用し、構成済みのしきい値を超えた場合にユーザーにアラートを送信できます。 また、ユーザーがしきい値を超えた場合にローミングを無効にするなど、さまざまな処理を行うようにサービスを構成することもできます。 Saaswedo コンソールでは、データの使用状況と監視情報を提供するレポートを利用することができます。 Intune で Saaswedo 通信経費管理サービスを使用する前に、Saaswedo コンソールと Intune で設定を構成する必要があります。 Saaswedo サービスおよび Intune に対する接続はオンにする必要があります。 Saaswedo 側の接続が有効で Intune 側の接続が有効でない場合、Intune 側は通信を受信しますが、それを無視します。

次の Graph リソースを使用して、Intune での通信費を管理できます。  

- [通信経費の管理パートナー](intune-tem-telecomexpensemanagementpartner.md)
