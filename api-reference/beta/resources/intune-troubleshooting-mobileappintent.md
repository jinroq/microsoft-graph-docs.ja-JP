---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
ms.openlocfilehash: 52d704f19379e2ac6232a37926185fd5d78c2e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072295"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイスのモバイル アプリケーションのステータスを示します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|使用可能|0|Available|
|送出|1|利用できません。|
|requiredInstall|2|必要なインストール|
|requiredUninstall|3|必要なアンインストール|
|requiredAndAvailableInstall|4|RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5|AvailableInstallWithoutEnrollment|
|除外|6|除外|





