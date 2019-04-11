---
title: mobileAppIntent 列挙型
description: デバイス上のモバイルアプリの状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785917"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス上のモバイルアプリの状態を示します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|使用可能|.0|Available|
|notavailable|1-d|インストールしない|
|requiredinstall|pbm-2|必要なインストール|
|requireduninstall|1/3|必要なアンインストール|
|requiredandのインストール|2/4|requiredandのインストール|
|登録がありません。|5|登録がありません。|
|削除|シックス|除外|



