# <a name="configuring-the-invitation-message"></a><span data-ttu-id="466b3-101">招待メッセージの構成</span><span class="sxs-lookup"><span data-stu-id="466b3-101">Configuring the invitation message</span></span>

<span data-ttu-id="466b3-102">invitedUserMessageInfo オブジェクトでは、[招待](invitation.md)メッセージを構成できます。</span><span class="sxs-lookup"><span data-stu-id="466b3-102">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="466b3-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="466b3-103">Properties</span></span>
| <span data-ttu-id="466b3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="466b3-104">Property</span></span>     | <span data-ttu-id="466b3-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="466b3-105">Type</span></span>   |<span data-ttu-id="466b3-106">説明</span><span class="sxs-lookup"><span data-stu-id="466b3-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="466b3-107">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="466b3-107">ccRecipients</span></span>|<span data-ttu-id="466b3-108">[Recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="466b3-108">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="466b3-p101">招待メッセージの送信先にする必要がある追加の受信者。現在、サポートされている追加の受信者は 1 人のみです。</span><span class="sxs-lookup"><span data-stu-id="466b3-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="466b3-111">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="466b3-111">customizedMessageBody</span></span>|<span data-ttu-id="466b3-112">String</span><span class="sxs-lookup"><span data-stu-id="466b3-112">String</span></span>|<span data-ttu-id="466b3-113">既定のメッセージを使用しない場合に送信するカスタマイズされたメッセージ本文。</span><span class="sxs-lookup"><span data-stu-id="466b3-113">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="466b3-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="466b3-114">messageLanguage</span></span>|<span data-ttu-id="466b3-115">String</span><span class="sxs-lookup"><span data-stu-id="466b3-115">String</span></span>|<span data-ttu-id="466b3-p102">既定のメッセージを送信する言語。customizedMessageBody が指定されている場合、このプロパティは無視され、メッセージは ustomizedMessageBody を使用して送信されます。言語書式は ISO 639 である必要があります。既定では ja-JP です。</span><span class="sxs-lookup"><span data-stu-id="466b3-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="466b3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="466b3-120">JSON representation</span></span>
<span data-ttu-id="466b3-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="466b3-121">Here is a JSON representation of the resource</span></span>

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
