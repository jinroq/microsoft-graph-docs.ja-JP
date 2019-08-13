---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザーアカウント制御設定に指定できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1e26ef18691f457be74d172f9a1fc1671248ca9d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369487"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>windowsUserAccountControlSettings 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows ユーザーアカウント制御設定に指定できる値。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザー定義、既定値、意図的ではありません。|
|常に通知|1-d|常に通知します。|
|notifyOnAppChanges|pbm-2|アプリの変更について通知します。|
|Notifyonappのすべての非追加暗転|1/3|デスクトップを暗転せずに、アプリの変更について通知します。|
|neverNotify|2/4|通知しません。|



