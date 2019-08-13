---
title: remoteAssistanceOnboardingStatus 列挙型
description: 現在の TeamViewer connector の状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bd51496000bce906457b4ea03586a41c46e2e426
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308149"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>remoteAssistanceOnboardingStatus 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

現在の TeamViewer connector の状態

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|notOnboarded|.0|アクティブな TeamViewer connector が構成されていない場合、またはアクティブである場合に報告される状態|
|契約|1-d|システムが TeamViewer 接続を開始したときに報告された状態ですが、サービスはまだコネクタの確認を完了していません。|
|利用|pbm-2|システムが TeamViewer を使用してアカウント情報を正常に交換し、クライアントとのリモートアシスタンスセッションを開始できるようになったときに報告された状態。|



