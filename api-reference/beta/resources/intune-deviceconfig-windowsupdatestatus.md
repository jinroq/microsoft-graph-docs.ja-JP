---
title: windowsUpdateStatus 列挙型
description: ビジネス構成デバイスの状態に関する Windows update
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7549fb77cf5a9f7c3014192d5524019323405f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154160"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス構成デバイスの状態に関する Windows update

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|upToDate|.0|保留中の更新はありません。保留中の再起動更新プログラムはありません。更新は失敗しています。|
|pendinginstallation|1-d|承認されていない更新プログラムが含まれている保留中の更新プログラムがあります。 保留中の再起動更新はありません。更新は失敗しません。|
|pendingreboot|pbm-2|再起動が必要な更新プログラムがあります。 失敗した更新はありません。|
|フェール|1/3|デバイスにインストールできなかった更新プログラムがあります。|




