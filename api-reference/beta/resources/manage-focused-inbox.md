---
title: 優先受信トレイを管理する
description: '重要なメッセージを表示することにより、フォーカスのある受信トレイ、 `Focused` 、受信トレイで受信トレイのメッセージの残りの部分のタブ、 `Other` ] タブ。分類システム '
localization_priority: Normal
ms.openlocfilehash: 5ee5d5f9dd48faa7d0590cbbc6dfda39d8f117e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529251"
---
# <a name="manage-focused-inbox"></a><span data-ttu-id="ef562-103">優先受信トレイを管理する</span><span class="sxs-lookup"><span data-stu-id="ef562-103">Manage Focused Inbox</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef562-p101">優先受信トレイでは、受信トレイの `Focused` タブに重要メッセージを表示し、その他の受信トレイのメッセージを `Other` タブに表示します。システム主体の分類方法によって、既定の方法で受信トレイのメッセージが整理されます。ユーザー インターフェイスまたはプログラムを介して、時間の経過によってシステムを修正し、学習させることができます。使用頻度が増えるほど、システムは、受信したメッセージの重要性をより高い精度で予想できるようになります。</span><span class="sxs-lookup"><span data-stu-id="ef562-p101">Focused Inbox allows you to view important messages in the `Focused` tab of the Inbox, and the rest of the Inbox messages in the `Other` tab. The classification system initially organizes Inbox messages in a default way. You can correct and train the system over time through the user interface or programmatically. The more you use it, the better the system can infer which incoming message as important.</span></span>

<span data-ttu-id="ef562-p102">プログラム レベルでは、優先受信トレイ REST API は指定のユーザー メッセージで機能し、メッセージごとの **inferenceClassification** プロパティをサポートします。使用可能な値は `Focused` と `Other` であり、ユーザーがそれぞれのメッセージの重要性をどのように見なしているかを示しています。システムがメッセージを分類する方法を修正するには [該当するメッセージの inferenceClassification プロパティを更新します](../api/message-update.md)。時間の経過と共に、これらの修正によっても、メッセージの分類システムが改善されます。</span><span class="sxs-lookup"><span data-stu-id="ef562-p102">At the programmatic level, the Focused Inbox REST API works on the specified user's messages, and supports an **inferenceClassification** property for each message. The possible values are `Focused` and `Other`, which indicate whether the user considers that message as, respectively, more important and less important. To correct how the system classifies a message, [update the inferenceClassification property of that message](../api/message-update.md). Over time, these corrections also train the message classification system.</span></span>

<span data-ttu-id="ef562-p103">優先受信トレイ REST API では、オーバーライドを作成することもできます。それぞれのオーバーライドは [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) インスタンスで表され、分類システムが常に一貫した方法 (常に "優先" または "その他") で、それまでに学習した方法に関係なく、特定の送信者からのメッセージを指定するように指示するものです。指定したユーザーのオーバーライドを[作成](../api/inferenceclassification-post-overrides.md)、[一覧表示](../api/inferenceclassification-list-overrides.md)、[更新](../api/inferenceclassificationoverride-update.md)、[削除](../api/inferenceclassificationoverride-delete.md)することができます。そのユーザーのオーバーライド (ある場合) は、**inferenceClassificationOverride** インスタンスのコレクションである、**inferenceClassification** ナビゲーション プロパティでアクセスできます。オーバーライドでは、ユーザーは受信メッセージの分類をさらに細かく制御でき、分類システムの信頼性を高めることができます。</span><span class="sxs-lookup"><span data-stu-id="ef562-p103">The Focused Inbox REST API also lets you create overrides. Each override, represented by an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance, is an instruction for the classification system to always designate messages from a specific sender in a consistent way (i.e., always as "Focused" or always as "Other"), regardless of any previously learned approach. You can [create](../api/inferenceclassification-post-overrides.md), [list](../api/inferenceclassification-list-overrides.md), [update](../api/inferenceclassificationoverride-update.md) and [delete](../api/inferenceclassificationoverride-delete.md) overrides for the specified user. That user's overrides, if any, are accessible in an **inferenceClassification** navigation property, which is a collection of **inferenceClassificationOverride** instances. Overrides allow a user more control over the classification of incoming messages, and build greater trust of the classification system.</span></span>

<span data-ttu-id="ef562-p104">分類システムでは受信トレイの受信メッセージについてのみ分類を学習し、適用することに注意してください。その他のフォルダーにあるメッセージは、既定で "優先" になっています。オーバーライドの設定は、今後、受信トレイに入ってくるメッセージに反映され、オーバーライドでは、受信トレイを含むフォルダーにある既存のメッセージの **inferenceClassification** プロパティは変更されません。</span><span class="sxs-lookup"><span data-stu-id="ef562-p104">Note that the classification system learns and applies classification only on incoming messages in the Inbox. Messages in other folders are by default "Focused". Setting up an override affects future messages arriving in the Inbox; the override doesn't modify the **inferenceClassification** property in existing messages in any folder including the Inbox.</span></span>

## <a name="focused-inbox-api"></a><span data-ttu-id="ef562-119">優先受信トレイ API</span><span class="sxs-lookup"><span data-stu-id="ef562-119">Focused Inbox API</span></span>

<span data-ttu-id="ef562-120">**メッセージ分類システムの記憶**</span><span class="sxs-lookup"><span data-stu-id="ef562-120">**Training the message classification system**</span></span>

[<span data-ttu-id="ef562-121">メッセージの inferenceClassification プロパティの更新</span><span class="sxs-lookup"><span data-stu-id="ef562-121">Update the inferenceClassification property of a message</span></span>](../api/message-update.md)


<span data-ttu-id="ef562-122">**オーバーライドを使用した、送信者ごとに一貫した分類**</span><span class="sxs-lookup"><span data-stu-id="ef562-122">**Using overrides to classify consistently per sender**</span></span>

<span data-ttu-id="ef562-123">[送信者のオーバーライドを作成する](../api/inferenceclassification-post-overrides.md) | [ユーザーのすべてのオーバーライドを一覧表示する](../api/inferenceclassification-list-overrides.md) |</span><span class="sxs-lookup"><span data-stu-id="ef562-123">[Create an override for a sender](../api/inferenceclassification-post-overrides.md) | [List all user overrides](../api/inferenceclassification-list-overrides.md) |</span></span>

<span data-ttu-id="ef562-124">[送信者のオーバーライドを更新する](../api/inferenceclassificationoverride-update.md) | [送信者のオーバーライドを削除する](../api/inferenceclassificationoverride-delete.md)</span><span class="sxs-lookup"><span data-stu-id="ef562-124">[Update an override for a sender](../api/inferenceclassificationoverride-update.md) | [Delete a sender override](../api/inferenceclassificationoverride-delete.md)</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/manage-focused-inbox.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
