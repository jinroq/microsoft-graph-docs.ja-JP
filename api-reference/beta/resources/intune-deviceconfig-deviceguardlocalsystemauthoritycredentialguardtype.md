---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: キラーの資格情報の設定で使用できる値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d8643744e1f5c36cf6c620ac85a6a99c9a77548
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398094"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a>deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キラーの資格情報の設定で使用できる値です。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|UEFI ロックせずに以前設定されている場合リモート資格情報の保護をオフにします。|
|enableWithUEFILock|1|UEFI ロックで資格情報の保護をオンにします。|
|enableWithoutUEFILock|2|UEFI ロックせず資格情報の保護をオンにします。|




