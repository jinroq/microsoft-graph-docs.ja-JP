---
title: windowsUpdateStatus 列挙型
description: ビジネス構成のデバイスの状態の windows を更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431654"
---
# <a name="windowsupdatestatus-enum-type"></a>windowsUpdateStatus 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス構成のデバイスの状態の windows を更新します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|古く|0|保留中の更新プログラム、更新プログラムの再起動や障害が発生した更新保留中の不要はありません。|
|pendingInstallation|1|保留中の承認されていない更新プログラムを含むインストールの更新プログラムがあります。 再起動の保留中の更新はありません、ない障害が発生した更新プログラムがあります。|
|pendingReboot|2|再起動を必要とする更新プログラムがあります。 更新が失敗したことがありません。|
|失敗しました。|3|デバイスのインストールに失敗した更新プログラムがあります。|




