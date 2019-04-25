---
title: managementstate 列挙型
description: Microsoft Intune でのデバイスの管理状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05dc0db1ecbe88616ca36db82bad2081b4133e3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521293"
---
# <a name="managementstate-enum-type"></a>managementstate 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Intune でのデバイスの管理状態。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|対象|.0|デバイスが管理下にある|
|retirePending|1 |廃棄コマンドは、デバイス上および管理からの登録取り消しプロセス中に発生します。|
|retireFailed|2 |デバイスでのリタイアコマンドが失敗しました|
|wipepending|3 |ワイプコマンドがデバイス上で発生していて、管理からの登録取り消しプロセスである|
|wipefailed|4 |デバイスでワイプコマンドが失敗しました|
|正常|5 |デバイスに問題があります。|
|deletepending|6 |デバイスで削除コマンドが発生しています |
|retireIssued|7 |デバイスに対して、廃棄コマンドが発行されました|
|wipeissued 済み|8 |デバイスに対してワイプコマンドが発行されました|
|wipeCanceled|9 |このデバイスのワイプコマンドは取り消されました|
|retireCanceled|10  |このデバイスの廃棄コマンドは取り消されました|
|た|11 |デバイスが検出されますが、完全に登録されていません。|





