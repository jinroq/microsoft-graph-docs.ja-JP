---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a807e89ec949c2c48f04af46b26f43b393cc4b0a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419262"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




