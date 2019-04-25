---
title: 通話における IVR シナリオ
description: 次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aed30bc5ad109dc3f21d381f4d6b04e087a779a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535569"
---
# <a name="ivr-scenarios-in-calls"></a>通話における IVR シナリオ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

次に示す対話式音声応答 (IVR) シナリオでは、Microsoft Graph の呼び出し元 api がサポートしています。

- 音声ガイダンスを再生する-たとえば、カスタマーサービスエージェントのキューに通話が配置された場合です。
- record-たとえば、発信者の音声を録音する場合、通常は、オプションを含むプロンプトが表示された後に録音します。
- [トーン] (たとえば、発信者が選択した DTMF トーンを知る必要がある場合)、通常は音声プロンプトを聞きます。
- メディア処理をキャンセルします。たとえば、再生プロンプトや、処理中の可能性があるレコード操作を取り消す場合です。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-ivr-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
