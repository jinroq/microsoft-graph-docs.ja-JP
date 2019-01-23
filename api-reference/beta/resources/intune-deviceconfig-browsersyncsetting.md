---
title: browserSyncSetting 列挙型
description: Allow(Not Configured) または prevent(Block) がマイクロソフトのエッジのブラウザーの設定の同期します。 防止するオプションはデバイス間で同期しますが、ユーザーのオーバーライドを許可します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dce2b82b1eea5e4b06ed0f6949ba6a403b073a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431590"
---
# <a name="browsersyncsetting-enum-type"></a>browserSyncSetting 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Allow(Not Configured) または prevent(Block) がマイクロソフトのエッジのブラウザーの設定の同期します。 防止するオプションはデバイス間で同期しますが、ユーザーのオーバーライドを許可します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notConfigured|0|既定 – 複数のデバイスのブラウザーの設定の同期を許可します。|
|blockedWithUserOverride|1|複数のユーザーのデバイスのブラウザーの設定の同期を防ぐため、設定のユーザーの上書きを許可します。|
|ブロック|2|絶対に複数のユーザーのデバイスのブラウザーの設定の同期を防ぐためです。|




