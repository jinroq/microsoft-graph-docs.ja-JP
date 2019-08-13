---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 41a6d23e42d263dd8241e960af693450ac0a7c3d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369508"
---
# <a name="windowsupdatetype-enum-type"></a>windowsUpdateType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

更新プログラムを受信するブランチデバイス

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|自分のもの|.0|ユーザーがを設定できるようにします。|
|すべての|1-d|半期チャネル (対象指定)。 デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。|
|businessReadyOnly|pbm-2|半期チャネル デバイスは、半期チャネルから機能の更新を取得します。|
|windowsInsiderBuildFast|1/3|Windows Insider ビルド-Fast|
|windowsInsiderBuildSlow|2/4|Windows Insider ビルド-低速|
|windowsInsiderBuildRelease|5|Windows Insider ビルドをリリースする|



