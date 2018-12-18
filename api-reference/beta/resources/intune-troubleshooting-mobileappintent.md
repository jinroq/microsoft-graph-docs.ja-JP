---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
author: tfitzmac
ms.openlocfilehash: 0a230279a947ab60314a53872670fff871eff745
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347230"
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





