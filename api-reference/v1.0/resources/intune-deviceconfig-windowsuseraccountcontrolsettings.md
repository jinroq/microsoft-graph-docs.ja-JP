---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 478e525847f7f6519b3bd2cb230ce2657b409f9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503635"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 列挙型

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ユーザーアカウント制御設定に指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|常に通知|1 |常に通知します。|
|notifyonappchanges|2 |アプリの変更について通知します。|
|notifyonappのすべての非追加暗転|3 |デスクトップを暗転せずに、アプリの変更について通知します。|
|neverNotify|4 |通知しません。|



