---
title: 'user: findMeetingTimes'
description: 会議の時間と開催者と出席者の可用性、およびパラメーターとして指定された時間や場所の制約に基づいて場所をお勧めします。
ms.openlocfilehash: 7ee6794041310d031f257bb83714de57f4af0cee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020404"
---
# <a name="user-findmeetingtimes"></a><span data-ttu-id="f5f38-103">user: findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="f5f38-103">user: findMeetingTimes</span></span>
<span data-ttu-id="f5f38-104">会議の時間と開催者と出席者の可用性、およびパラメーターとして指定された時間や場所の制約に基づいて場所をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f5f38-104">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints specified as parameters.</span></span>

<span data-ttu-id="f5f38-p101">**findMeetingTimes** が会議提案を返すことができない場合は、応答で、**emptySuggestionsReason** プロパティに理由が示されます。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** を再度呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p101">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>


## <a name="permissions"></a><span data-ttu-id="f5f38-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f5f38-107">Permissions</span></span>
<span data-ttu-id="f5f38-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5f38-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5f38-110">Permission type</span></span>      | <span data-ttu-id="f5f38-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5f38-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5f38-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5f38-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5f38-113">Calendars.Read.Shared、Calendars.ReadWrite.Shared</span><span class="sxs-lookup"><span data-stu-id="f5f38-113">Calendars.Read.Shared, Calendars.ReadWrite.Shared</span></span>    |
|<span data-ttu-id="f5f38-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5f38-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5f38-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5f38-115">Not supported.</span></span>    |
|<span data-ttu-id="f5f38-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5f38-116">Application</span></span> | <span data-ttu-id="f5f38-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5f38-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5f38-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5f38-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a><span data-ttu-id="f5f38-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5f38-119">Request headers</span></span>
| <span data-ttu-id="f5f38-120">名前</span><span class="sxs-lookup"><span data-stu-id="f5f38-120">Name</span></span>       | <span data-ttu-id="f5f38-121">値</span><span class="sxs-lookup"><span data-stu-id="f5f38-121">Value</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f5f38-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5f38-122">Authorization</span></span>  | <span data-ttu-id="f5f38-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5f38-125">優先: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f5f38-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f5f38-p104">応答として "太平洋標準時" などの特定のタイム ゾーンを表す文字列です。省略可能。このヘッダーが指定されていない場合は、UTC が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p104">A string representing a specific time zone for the response, for example, "Pacific Standard Time". Optional. UTC is used if this header is not specified.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5f38-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5f38-129">Request body</span></span>
<span data-ttu-id="f5f38-p105">サポートされているすべてのパラメーターは以下のとおりです。シナリオに応じて、要求本文で必要な各パラメーターの JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p105">All the supported parameters are listed below. Depending on your scenario, specify a JSON object for each of the necessary parameters in the request body.</span></span> 


| <span data-ttu-id="f5f38-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f5f38-132">Parameter</span></span>    | <span data-ttu-id="f5f38-133">型</span><span class="sxs-lookup"><span data-stu-id="f5f38-133">Type</span></span>   |<span data-ttu-id="f5f38-134">説明</span><span class="sxs-lookup"><span data-stu-id="f5f38-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5f38-135">attendees</span><span class="sxs-lookup"><span data-stu-id="f5f38-135">attendees</span></span>|<span data-ttu-id="f5f38-136">[attendeeBase](../resources/attendeebase.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f5f38-136">[attendeeBase](../resources/attendeebase.md) collection</span></span>|<span data-ttu-id="f5f38-p106">会議の出席者またはリソースのコレクションです。findMeetingTimes では個人の出席者が常に必要であると仮定されているため、個人として `required`、対応する **type** プロパティのリソースとして `resource` を指定します。コレクションを空にすると、**findMeetingTimes** は開催者のみの空き時間帯を検索します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p106">A collection of attendees or resources for the meeting. Since findMeetingTimes assumes that any attendee who is a person is always required, specify `required` for a person and `resource` for a resource in the corresponding **type** property. An empty collection causes **findMeetingTimes** to look for free time slots for only the organizer. Optional.</span></span>|
|<span data-ttu-id="f5f38-141">isOrganizerOptional</span><span class="sxs-lookup"><span data-stu-id="f5f38-141">isOrganizerOptional</span></span>|<span data-ttu-id="f5f38-142">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f5f38-142">Edm.Boolean</span></span>|<span data-ttu-id="f5f38-p107">開催者が必ずしも出席する必要がない場合は、`True` を指定します。既定値は `false` です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p107">Specify `True` if the organizer doesn't necessarily have to attend. The default is `false`. Optional.</span></span>|
|<span data-ttu-id="f5f38-146">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f5f38-146">locationConstraint</span></span>|[<span data-ttu-id="f5f38-147">locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f5f38-147">locationConstraint</span></span>](../resources/locationconstraint.md)|<span data-ttu-id="f5f38-p108">会議の場所の提案が必要かどうか、または会議のみが開催できる特定の場所があるか、など、会議の場所に関する開催者の要件。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p108">The organizer's requirements about the meeting location, such as whether a suggestion for a meeting location is required, or there are specific locations only where the meeting can take place. Optional.</span></span>|
|<span data-ttu-id="f5f38-150">maxCandidates</span><span class="sxs-lookup"><span data-stu-id="f5f38-150">maxCandidates</span></span>|<span data-ttu-id="f5f38-151">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f5f38-151">Edm.Int32</span></span>|<span data-ttu-id="f5f38-p109">返される会議時間の提案の最大数です。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p109">The maximum number of meeting time suggestions to be returned. Optional.</span></span>|
|<span data-ttu-id="f5f38-154">meetingDuration</span><span class="sxs-lookup"><span data-stu-id="f5f38-154">meetingDuration</span></span>|<span data-ttu-id="f5f38-155">Edm.Duration</span><span class="sxs-lookup"><span data-stu-id="f5f38-155">Edm.Duration</span></span>|<span data-ttu-id="f5f38-p110">[ISO8601](https://www.iso.org/iso/iso8601) 形式で示された会議の長さです。たとえば、1 時間は 'PT1H' として示され、このとき 'P' は期間の指定子、'T' は時刻の指定子、'H' は時間の指定子です。期間の分を示すには M を使用します。たとえば、2 時間 30 分は 'PT2H30M' になります。会議の期間を指定しない場合、**findMeetingTimes** は既定値の 30 分を使用します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p110">The length of the meeting, denoted in [ISO8601](https://www.iso.org/iso/iso8601) format. For example, 1 hour is denoted as 'PT1H', where 'P' is the duration designator, 'T' is the time designator, and 'H' is the hour designator. Use M to indicate minutes for the duration; for example, 2 hours and 30 minutes would be 'PT2H30M'. If no meeting duration is specified, **findMeetingTimes** uses the default of 30 minutes. Optional.</span></span>|
|<span data-ttu-id="f5f38-161">minimumAttendeePercentage</span><span class="sxs-lookup"><span data-stu-id="f5f38-161">minimumAttendeePercentage</span></span>|<span data-ttu-id="f5f38-162">Edm.Double</span><span class="sxs-lookup"><span data-stu-id="f5f38-162">Edm.Double</span></span>| <span data-ttu-id="f5f38-p111">応答で返される時間帯に最低限要求される[確度](#the-confidence-of-a-meeting-suggestion)です。割合 ( %) の値 (0 から 100 まで)。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p111">The minimum required [confidence](#the-confidence-of-a-meeting-suggestion) for a time slot to be returned in the response. It is a % value ranging from 0 to 100. Optional.</span></span>|
|<span data-ttu-id="f5f38-166">returnSuggestionReasons</span><span class="sxs-lookup"><span data-stu-id="f5f38-166">returnSuggestionReasons</span></span>|<span data-ttu-id="f5f38-167">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f5f38-167">Edm.Boolean</span></span>|<span data-ttu-id="f5f38-p112">**SuggestionReason** プロパティで各会議提案の理由を返すには、`True` を指定します。既定値は `false` であり、そのプロパティを返しません。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p112">Specify `True` to return a reason for each meeting suggestion in the **suggestionReason** property. The default is `false` to not return that property. Optional.</span></span>|
|<span data-ttu-id="f5f38-171">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f5f38-171">timeConstraint</span></span>|[<span data-ttu-id="f5f38-172">timeConstraint</span><span class="sxs-lookup"><span data-stu-id="f5f38-172">timeConstraint</span></span>](../resources/timeconstraint.md)|<span data-ttu-id="f5f38-p113">会議の性質 (**activityDomain** プロパティ) と可能な会議の時間帯 (**timeSlots** property) を含めることのできる時間制限。このパラメーターを指定しない場合、**findMeetingTimes** が **activityDomain** を `work` と仮定します。省略可能。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p113">Any time restrictions for a meeting, which can include the nature of the meeting (**activityDomain** property) and possible meeting time periods (**timeSlots** property). **findMeetingTimes** assumes **activityDomain** as `work` if you don't specify this parameter. Optional.</span></span>|

<span data-ttu-id="f5f38-176">次の表では、 **timeConstraint**パラメーターで指定できます**activityDomain**の制限について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-176">The following table describes the **activityDomain** restrictions you can further specify in the **timeConstraint** parameter.</span></span>

|<span data-ttu-id="f5f38-177">activityDomain 値</span><span class="sxs-lookup"><span data-stu-id="f5f38-177">activityDomain value</span></span>|<span data-ttu-id="f5f38-178">会議の時間の候補</span><span class="sxs-lookup"><span data-stu-id="f5f38-178">Suggestions for meeting times</span></span>|
|:-----|:-----|
|<span data-ttu-id="f5f38-179">作業</span><span class="sxs-lookup"><span data-stu-id="f5f38-179">work</span></span>| <span data-ttu-id="f5f38-p114">ユーザーの予定表の構成で定義された稼働時間 (ユーザーまたは管理者がカスタマイズできる) の範囲内で候補が提案されます。既定の稼働時間は、月曜日から金曜日の午前 8 時から午後 5 時 (メールボックスに設定されたタイム ゾーンでの時刻) です。**activityDomain** を指定しない場合、これが既定値です。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p114">Suggestions are within the user's work hours which are defined in the user’s calendar configuration and can be customized by the user or administrator. The default work hours are Monday to Friday, 8am to 5pm in the time zone set for the mailbox. This is the default value if no **activityDomain** is specified.</span></span> |
|<span data-ttu-id="f5f38-183">personal</span><span class="sxs-lookup"><span data-stu-id="f5f38-183">personal</span></span>| <span data-ttu-id="f5f38-p115">ユーザーの稼働時間の範囲内と、土曜日と日曜日の範囲内で候補が提案されます。既定では、月曜日から日曜日の午前 8 時から午後 5 時 (メールボックスに設定されたタイム ゾーンでの時刻) です。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p115">Suggestions are within the user's work hours, and Saturday and Sunday. The default is Monday to Sunday, 8am to 5pm, in the time zone setting for the mailbox.</span></span>|
|<span data-ttu-id="f5f38-186">Unrestricted</span><span class="sxs-lookup"><span data-stu-id="f5f38-186">unrestricted</span></span> | <span data-ttu-id="f5f38-187">任意の曜日の任意の時刻から候補が提案されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-187">Suggestions can be from all hours of a day, all days of a week.</span></span>|
|<span data-ttu-id="f5f38-188">不明</span><span class="sxs-lookup"><span data-stu-id="f5f38-188">unknown</span></span> | <span data-ttu-id="f5f38-p116">将来的に使われなくなりますので、この値は使わないでください。現在の動作は、`work` と同じです。`work`、`personal` または `unrestricted` を使用するように、既存のコードを適宜変更します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p116">Do not use this value as it will be deprecated in the future. Currently behaves the same as `work`. Change any existing code to use `work`, `personal` or `unrestricted` as appropriate.</span></span>


<span data-ttu-id="f5f38-p117">指定したパラメーターに基づいて、**findMeetingTimes** は開催者と出席者の標準として設定されている予定表で空き時間状態を確認します。アクションは、開催できる可能性が最も高い会議の日時を計算し、会議の提案を返します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p117">Based on the specified parameters,**findMeetingTimes** checks the free/busy status in the primary calendars of the organizer and attendees. The action calculates the best possible meeting times, and returns any meeting suggestions.</span></span>

## <a name="response"></a><span data-ttu-id="f5f38-194">応答</span><span class="sxs-lookup"><span data-stu-id="f5f38-194">Response</span></span>

<span data-ttu-id="f5f38-195">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に入った [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-195">If successful, this method returns `200 OK` response code and a [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) in the response body.</span></span> 

<span data-ttu-id="f5f38-p118">**meetingTimeSuggestionsResult** には、会議提案のコレクションと **emptySuggestionsReason** プロパティが含まれます。各提案は、[meetingTimeSuggestion](../resources/meetingtimesuggestion.md) として定義され、出席者の参加の確度について、平均で 50% または**minimumAttendeePercentage** パラメーターで指定した特定の割合 (%) が付されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p118">A **meetingTimeSuggestionsResult** includes a collection of meeting suggestions and an **emptySuggestionsReason** property. Each suggestion is defined as a [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), with attendees having on the average a confidence level of 50% to attend, or a specific % that you have specified in the **minimumAttendeePercentage** parameter.</span></span> 

<span data-ttu-id="f5f38-198">既定では、会議の日時についての各提案は UTC で返されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-198">By default, each meeting time suggestion is returned in UTC.</span></span> 

<span data-ttu-id="f5f38-p119">**findMeetingTimes** が会議提案を返すことができない場合は、応答で、**emptySuggestionsReason** プロパティに理由が示されます。この値に基づいて、パラメーターをさらに調整して、**findMeetingTimes** を再度呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p119">If **findMeetingTimes** cannot return any meeting suggestions, the response would indicate a reason in the **emptySuggestionsReason** property. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

### <a name="the-confidence-of-a-meeting-suggestion"></a><span data-ttu-id="f5f38-201">会議の提案の確実性</span><span class="sxs-lookup"><span data-stu-id="f5f38-201">The confidence of a meeting suggestion</span></span>

<span data-ttu-id="f5f38-202">**meetingTimeSuggestion** の **confidence** プロパティの範囲は 0% から 100% で、各個人の空き時間状態に基づいて会議に出席するすべての出席者の見込みを表します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-202">The **confidence** property of a **meetingTimeSuggestion** ranges from 0% to 100%, and represents the chance that all the attendees attend the meeting, based on each of their individual free/busy status:</span></span>

- <span data-ttu-id="f5f38-203">各出席者に関する、指定の会議期間の空き状態で、確実に出席する場合は 100%、不明な状態は 49%、忙しい場合には 0% です。</span><span class="sxs-lookup"><span data-stu-id="f5f38-203">For each attendee, a free status for a specified meeting time period corresponds to 100% chance of attendance, unknown status 49%, and busy status 0%.</span></span>
- <span data-ttu-id="f5f38-204">会議時間の提案の確実性は、指定された対象会議のすべての出席者の出席見込みの平均によって算出されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-204">The confidence of a meeting time suggestion is computed by averaging the chance of attendance over all the attendees specified for that meeting.</span></span>
- <span data-ttu-id="f5f38-p120">**findMeetingTimes** の **minimumAttendeePercentage** オプション パラメーターを使用して、少なくとも特定の信頼度の会議の時間帯のみが返されるように指定することができます。たとえば、すべての出席者が出席する見込みが 80% 以上ある提案のみを行う場合は、80% の **minimumAttendeePercentage** を指定できます。**minimumAttendeePercentage** を指定しない場合は、**findMeetingTimes** は 50% の値を前提とします。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p120">You can use the **minimumAttendeePercentage** optional parameter for **findMeetingTimes** to specify only meeting time suggestions of at least certain confidence level should be returned. For example, you can specify a **minimumAttendeePercentage** of 80% if you want only suggestions that have an 80% chance or more that all the attendees are attending. If you do not specify **minimumAttendeePercentage**, **findMeetingTimes** assumes a value of 50%.</span></span>
- <span data-ttu-id="f5f38-p121">会議時間の提案が複数ある場合、**findMeetingTimes** アクションは、算出した確実性が高い方から順番に提案を並べて示します。確実性が同じ提案がある場合には、時系列で提案を並べて示します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p121">If there are multiple meeting time suggestions, the **findMeetingTimes** action first orders the suggestions by their computed confidence value from high to low. If there are suggestions with the same confidence, the action then orders these suggestions chronologically.</span></span>

<span data-ttu-id="f5f38-210">たとえば、提案の会議時間に次の空き時間状態の 3 人の出席者がいるとします。</span><span class="sxs-lookup"><span data-stu-id="f5f38-210">As an example, if a meeting time suggestion involves 3 attendees with the following free/busy status:</span></span>

|<span data-ttu-id="f5f38-211">**出席者**</span><span class="sxs-lookup"><span data-stu-id="f5f38-211">**Attendee**</span></span>|<span data-ttu-id="f5f38-212">**空き時間状態**</span><span class="sxs-lookup"><span data-stu-id="f5f38-212">**Free/busy status**</span></span>|<span data-ttu-id="f5f38-213">**出席見込み (%)**</span><span class="sxs-lookup"><span data-stu-id="f5f38-213">**% Chance of attendance**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f5f38-214">Dana</span><span class="sxs-lookup"><span data-stu-id="f5f38-214">Dana</span></span> | <span data-ttu-id="f5f38-215">空き</span><span class="sxs-lookup"><span data-stu-id="f5f38-215">Free</span></span> | <span data-ttu-id="f5f38-216">100%</span><span class="sxs-lookup"><span data-stu-id="f5f38-216">100%</span></span> |
|<span data-ttu-id="f5f38-217">John</span><span class="sxs-lookup"><span data-stu-id="f5f38-217">John</span></span> | <span data-ttu-id="f5f38-218">不明</span><span class="sxs-lookup"><span data-stu-id="f5f38-218">Unknown</span></span> | <span data-ttu-id="f5f38-219">49%</span><span class="sxs-lookup"><span data-stu-id="f5f38-219">49%</span></span> |
|<span data-ttu-id="f5f38-220">Samantha</span><span class="sxs-lookup"><span data-stu-id="f5f38-220">Samantha</span></span> | <span data-ttu-id="f5f38-221">多忙</span><span class="sxs-lookup"><span data-stu-id="f5f38-221">Busy</span></span> | <span data-ttu-id="f5f38-222">0%</span><span class="sxs-lookup"><span data-stu-id="f5f38-222">0%</span></span> |

<span data-ttu-id="f5f38-223">この場合、出席の平均見込みである会議時間の提案の信頼度は、(100% + 49% + 0%)/3 = 49.66% です。</span><span class="sxs-lookup"><span data-stu-id="f5f38-223">Then the confidence of the meeting time suggestion, which is the average chance of attendance, is (100% + 49% + 0%)/3 = 49.66%.</span></span>

<span data-ttu-id="f5f38-224">**findMeetingTimes** で 80% の **minimumAttendeePercentage** を指定すると、49.66% < 80% のため、操作では応答でこの時間の提案は返されません。</span><span class="sxs-lookup"><span data-stu-id="f5f38-224">If you specify a **minimumAttendeePercentage** of 80% in a **findMeetingTimes** operation, because 49.66% < 80%, the operation will not suggest this time in the response.</span></span>

## <a name="example"></a><span data-ttu-id="f5f38-225">例</span><span class="sxs-lookup"><span data-stu-id="f5f38-225">Example</span></span>

<span data-ttu-id="f5f38-226">次の例は、要求本文で次のパラメーターを指定して、あらかじめ決められた会議を開催する時間を検索し、各提案の理由を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f5f38-226">The following example shows how to find time to meet at a pre-determined location, and request a reason for each suggestion, by specifying the following parameters in the request body:</span></span>

- <span data-ttu-id="f5f38-227">**attendees**</span><span class="sxs-lookup"><span data-stu-id="f5f38-227">**attendees**</span></span>
- <span data-ttu-id="f5f38-228">**locationConstraint**</span><span class="sxs-lookup"><span data-stu-id="f5f38-228">**locationConstraint**</span></span>
- <span data-ttu-id="f5f38-229">**timeConstraint**</span><span class="sxs-lookup"><span data-stu-id="f5f38-229">**timeConstraint**</span></span>
- <span data-ttu-id="f5f38-230">**meetingDuration**</span><span class="sxs-lookup"><span data-stu-id="f5f38-230">**meetingDuration**</span></span>
- <span data-ttu-id="f5f38-231">**returnSuggestionReasons**</span><span class="sxs-lookup"><span data-stu-id="f5f38-231">**returnSuggestionReasons**</span></span>
- <span data-ttu-id="f5f38-232">**minimumAttendeePercentage**</span><span class="sxs-lookup"><span data-stu-id="f5f38-232">**minimumAttendeePercentage**</span></span>

<span data-ttu-id="f5f38-233">**findMeetingTimes** が任意の提案を返す場合は、**returnSuggestionReasons** パラメーターを設定することで、各提案の **SuggestionReason** プロパティの説明も取得できます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-233">By setting the **returnSuggestionReasons** parameter, you also get an explanation in the **suggestionReason** property for each suggestion, if **findMeetingTimes** returns any suggestion.</span></span>

<span data-ttu-id="f5f38-p122">既定では、要求は PST のタイム ゾーンの時間を指定し、応答は UTC で会議時間の提案を返すことに注意してください。PST を指定するのに、また応答の時間の値にも `Prefer: outlook.timezone` 要求ヘッダーを使うことができます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p122">Notice that the request specifies time in the PST time zone, and the response returns meeting time suggestions in UTC, by default. You can use the `Prefer: outlook.timezone` request header to specify PST as well for the time values in the response.</span></span>

##### <a name="request"></a><span data-ttu-id="f5f38-236">要求</span><span class="sxs-lookup"><span data-stu-id="f5f38-236">Request</span></span>
<span data-ttu-id="f5f38-237">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f5f38-237">Here is the example request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": "false",  
    "suggestLocation": "false",  
    "locations": [ 
      { 
        "resolveAvailability": "false",
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"unrestricted", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-17T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-19T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100.0
}
```

##### <a name="response"></a><span data-ttu-id="f5f38-238">応答</span><span class="sxs-lookup"><span data-stu-id="f5f38-238">Response</span></span>
<span data-ttu-id="f5f38-p123">応答の例を次に示します。メモ:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f5f38-p123">Here is an example response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 976

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T18:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        },
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-17T20:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-17T22:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/user-findmeetingtimes.md:
      Failed to parse any rows out of table with headers: |activityDomain value|Suggestions for meeting times|"
  ],
  "tocPath": ""
}-->