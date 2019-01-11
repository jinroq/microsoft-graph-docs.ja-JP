---
title: Microsoft Graph REST API v1.0 リファレンス
description: v1.0 エンドポイント用の Microsoft Graph REST API リファレンスへようこそ。
localization_priority: Priority
ms.openlocfilehash: 6e0dde56aae7857e9ae042f89ba5eb6b01737efa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829076"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a><span data-ttu-id="a33cc-103">Microsoft Graph REST API v1.0 リファレンス</span><span class="sxs-lookup"><span data-stu-id="a33cc-103">Microsoft Graph REST API v1.0 reference</span></span>

<span data-ttu-id="a33cc-104">v1.0 エンドポイント用の Microsoft Graph REST API リファレンスへようこそ。</span><span class="sxs-lookup"><span data-stu-id="a33cc-104">Welcome to Microsoft Graph REST API reference for the v1.0 endpoint.</span></span>

<span data-ttu-id="a33cc-105">v1.0 エンドポイントの API セット (`https://graph.microsoft.com/v1.0`) は、一般提供 (GA) ステータスで、顧客との厳密なレビューとフィードバック プロセスを経て、運用環境の実用的なニーズを満たすものとなっています。</span><span class="sxs-lookup"><span data-stu-id="a33cc-105">API sets on the v1.0 endpoint (`https://graph.microsoft.com/v1.0`) are in general availability (GA) status, and have gone through a rigorous review-and-feedback process with customers to meet practical, production needs.</span></span> <span data-ttu-id="a33cc-106">このエンドポイントの API の更新は、追加的なものであり、既存のアプリのシナリオを損なうものではありません。</span><span class="sxs-lookup"><span data-stu-id="a33cc-106">Updates to APIs on this endpoint are additive in nature and do not break existing app scenarios.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="a33cc-107">一般的なユース ケース</span><span class="sxs-lookup"><span data-stu-id="a33cc-107">Common use cases</span></span>

<span data-ttu-id="a33cc-108">Microsoft Graph では、単一の Microsoft Graph REST エンドポイントで公開されている異なるサービスのエンティティやリレーションシップのナビゲーションが簡単に行うことができます。</span><span class="sxs-lookup"><span data-stu-id="a33cc-108">The power of Microsoft Graph lies in easy navigation of entities and relationships across different services exposed on a single Microsoft Graph REST endpoint.</span></span>

<span data-ttu-id="a33cc-109">これらのサービスの多くは、[ユーザー](./resources/user.md)および[グループ](./resources/group.md)にとって、さまざまなシナリオを実現できるよう設計されています。</span><span class="sxs-lookup"><span data-stu-id="a33cc-109">A number of these services are designed to enable rich scenarios around a [user](./resources/user.md) and around a [group](./resources/group.md).</span></span>

### <a name="user-centric-use-cases-in-v10"></a><span data-ttu-id="a33cc-110">V1.0 でのユーザー中心のユース ケース</span><span class="sxs-lookup"><span data-stu-id="a33cc-110">User-centric use cases in v1.0</span></span>

1. <span data-ttu-id="a33cc-111">ユーザー (Lisa) の[プロファイルを取得](./api/user-get.md)し、[写真](./resources/profilephoto.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-111">[Get the profile](./api/user-get.md) and [photo](./resources/profilephoto.md) of a user, Lisa.</span></span>
2. <span data-ttu-id="a33cc-112">Azure Active Directory に保存されている [Lisa のマネージャーのプロファイル情報を取得](./api/user-list-manager.md)し、[直属の部下の ID](./api/user-list-directreports.md) を取得します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-112">[Get the profile information about Lisa's manager](./api/user-list-manager.md) and [IDs of her direct reports](./api/user-list-directreports.md), all stored in Azure Active Directory.</span></span>
3. <span data-ttu-id="a33cc-113">[OneDrive for Business 上で、Lisa のファイルにアクセス](./api/driveitem-list-children.md)し、最後にその[ファイル](./resources/driveitem.md)を更新した[ユーザー](./resources/identityset.md)を特定し、その人のプロファイルに移動します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-113">[Access Lisa's files on OneDrive for Business](./api/driveitem-list-children.md), find the [identity](./resources/identityset.md) of the last person who modified a [file](./resources/driveitem.md) there, and navigate to that person's profile.</span></span>
4. <span data-ttu-id="a33cc-114">Exchange Online 上の [Lisa の予定表にアクセス](./api/calendar-get.md)し、向こう 2 週間で [Lisa が彼女のチームとの会議に最適な時間を決定](./api/user-findmeetingtimes.md)します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-114">[Access Lisa's calendar](./api/calendar-get.md) on Exchange Online and [determine the best time for Lisa to meet with her team](./api/user-findmeetingtimes.md) in the next two weeks.</span></span>
5. <span data-ttu-id="a33cc-115">Lisa の予定表を[購読](./api/subscription-post-subscriptions.md)し、[変更履歴を記録](./api/event-delta.md)し、Lisa が会議に自分の時間の 80% 以上を費やしている場合に報告します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-115">[Subscribe to](./api/subscription-post-subscriptions.md) and [track changes](./api/event-delta.md) in Lisa's calendar, tell Lisa when she is spending more than 80% of her time in meetings.</span></span>
6. <span data-ttu-id="a33cc-116">Lisa が外出中のときに[自動応答を設定](./api/user-update-mailboxsettings.md#example)します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-116">[Set automatic replies](./api/user-update-mailboxsettings.md#example) when Lisa is away from the office.</span></span>
7. <span data-ttu-id="a33cc-117">コミュニケーション、コラボレーション、ビジネスのリレーションシップに基づいて、[Lisa にもっとも関連のある人物を取得](./api/user-list-people.md)します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-117">[Get the people who are most relevant to Lisa](./api/user-list-people.md), based on communication, collaboration, and business relationships.</span></span>
8. <span data-ttu-id="a33cc-118">Lisa の OneDrive for Business 上の Excel ファイルの、[グラフ](./resources/chart.md)から、最新の販売計画を取得します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-118">Get the latest sales projection from a [chart](./resources/chart.md) in an Excel file in Lisa's OneDrive for Business.</span></span>
9. <span data-ttu-id="a33cc-119">[Planner で Lisa に割り当てられているタスクを検索](./api/planneruser-list-tasks.md)します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-119">[Find the tasks assigned to Lisa in Planner](./api/planneruser-list-tasks.md).</span></span>

### <a name="office-365-group-use-cases-in-v10"></a><span data-ttu-id="a33cc-120">V1.0 での Office 365 グループのユース ケース</span><span class="sxs-lookup"><span data-stu-id="a33cc-120">Office 365 group use cases in v1.0</span></span>

1. <span data-ttu-id="a33cc-121">組織内の Office 365 グループに関するレポートを実行し、[グループのメンバー間の通信](./api/reportroot-getoffice365groupsactivitycounts.md)がもっとも多いグループを特定します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-121">Run a report on Office 365 groups in an organization and identify the group with the most [communication among group members](./api/reportroot-getoffice365groupsactivitycounts.md).</span></span>
2. <span data-ttu-id="a33cc-122">[この Office 365 グループの計画を検索](./api/plannergroup-list-plans.md)し、その計画の[タスクの割り当て](./resources/plannerassignments.md)を検索します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-122">[Find the plans of this Office 365 group](./api/plannergroup-list-plans.md), and the [assignment of tasks](./resources/plannerassignments.md) in that plan.</span></span>
3. <span data-ttu-id="a33cc-123">Office 365 グループ内で[新しい会話を開始](./api/group-post-conversations.md)し、メンバーがワークロードを共有するために[別のグループを作成する](./api/group-post-groups.md)かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-123">[Start a new conversation](./api/group-post-conversations.md) in the Office 365 group to determine if members want to [create another group](./api/group-post-groups.md) to share the workload.</span></span>
4. <span data-ttu-id="a33cc-124">グループの[既定のノートブックを取得](./api/notebook-get.md)し、調査の結果を記録する[新しいページを作成](./api/section-post-pages.md)します。</span><span class="sxs-lookup"><span data-stu-id="a33cc-124">[Get the default notebook](./api/notebook-get.md) for the group and [create a page](./api/section-post-pages.md) to note the outcome of the investigation.</span></span>

## <a name="other-api-versions"></a><span data-ttu-id="a33cc-125">その他の API バージョン</span><span class="sxs-lookup"><span data-stu-id="a33cc-125">Other API versions</span></span>

<span data-ttu-id="a33cc-126">現在、Microsoft Graph REST API には、- v1.0 とベータ版の 2 つのバージョンがあります。</span><span class="sxs-lookup"><span data-stu-id="a33cc-126">There are currently 2 versions of Microsoft Graph REST APIs - v1.0 and beta.</span></span>
<span data-ttu-id="a33cc-127">プレビューの状態にある新しいまたは拡張の API を検討する場合は 「[Microsoft Graph ベータ エンドポイント リファレンス](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-127">If you're interested in new or enhanced APIs that are still in preview status, see [Microsoft Graph beta endpoint reference](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta).</span></span> <span data-ttu-id="a33cc-128">プレビュー状態の API は今後変更される可能性があり、予告なしに既存のシナリオが動作しなくなる場合があることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-128">Be aware that APIs in preview status are subject to change, and may break existing scenarios without notice.</span></span> <span data-ttu-id="a33cc-129">ベータ版のエンドポイントの API に運用環境で依存関係を持たないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-129">Don't take a production dependency on APIs in the beta endpoint.</span></span>

<span data-ttu-id="a33cc-130">詳細については、「[バージョン管理とサポート](/graph/versioning-and-support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-130">Find more information about [versioning and support](/graph/versioning-and-support).</span></span>

## <a name="connect-with-us"></a><span data-ttu-id="a33cc-131">連絡方法</span><span class="sxs-lookup"><span data-stu-id="a33cc-131">Connect with us</span></span>

<span data-ttu-id="a33cc-132">Microsoft Graph に追加したい API や機能がある場合</span><span class="sxs-lookup"><span data-stu-id="a33cc-132">Are there additional APIs or features you'd like to see in Microsoft Graph?</span></span> <span data-ttu-id="a33cc-133">新しい機能のリクエストを [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632) に投稿してください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-133">Post new feature requests on [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).</span></span>

<span data-ttu-id="a33cc-134">既存の Microsoft Graph API に対するフィードバックがある場合</span><span class="sxs-lookup"><span data-stu-id="a33cc-134">Have feedback for existing Microsoft Graph APIs?</span></span> <span data-ttu-id="a33cc-135">[Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) から連絡してください。</span><span class="sxs-lookup"><span data-stu-id="a33cc-135">Connect with us on [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span></span>

<span data-ttu-id="a33cc-136">ご質問または Microsof を使用してコードのヘルプについて</span><span class="sxs-lookup"><span data-stu-id="a33cc-136">For questions or help with your code using Microsof</span></span>
