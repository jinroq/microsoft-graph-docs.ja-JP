---
title: 教育機関向け API の概要
description: Microsoft Graph の教育機関向け API は、教育のさまざまなシナリオに関係する情報によって Office 365 のリソースを拡張します。それには、学校、クラス、ユーザー (学生と教師)、課題、および提出に関する情報が含まれます。 これにより、学校やクラスルームのさまざまなシナリオのための教育関連リソースの統合ソリューションを容易に構築できます。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: c1a93242071f8ad1aa208ca3361f16d08c13d682
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778755"
---
# <a name="education-api-overview"></a><span data-ttu-id="638b2-104">教育機関向け API の概要</span><span class="sxs-lookup"><span data-stu-id="638b2-104">Education API overview</span></span>

<span data-ttu-id="638b2-105">Microsoft Graph の教育機関向け API は、教育のさまざまなシナリオに関係する情報によって Office 365 のリソースを拡張します。それには、学校、クラス、ユーザー (学生と教師)、課題、および提出に関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="638b2-105">The education API in Microsoft Graph enhances Office 365 resources with information that is relevant for education scenarios, including information about schools, classes, users (students and teachers), assignments, and submissions.</span></span> <span data-ttu-id="638b2-106">これにより、学校やクラスルームのさまざまなシナリオのための教育関連リソースの統合ソリューションを容易に構築できます。</span><span class="sxs-lookup"><span data-stu-id="638b2-106">This makes it easy for you to build solutions that integrate with educational resources for various school and classroom scenarios.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a><span data-ttu-id="638b2-107">教育のシナリオを統合する理由</span><span class="sxs-lookup"><span data-stu-id="638b2-107">Why integrate with education scenarios?</span></span>

### <a name="build-applications-that-are-aware-of-class-roster"></a><span data-ttu-id="638b2-108">クラスの名簿を認識するアプリケーションのビルド</span><span class="sxs-lookup"><span data-stu-id="638b2-108">Build applications that are aware of class roster</span></span>

<span data-ttu-id="638b2-109">教育関連のソフトウェア開発者の多くは、クラス名簿がアプリケーション実行に必要な情報の重要な部分の 1 つであるが、多くの場合は学校の学生情報システム (SIS) の内部にしまい込まれているという事実に早い段階で気付いています。</span><span class="sxs-lookup"><span data-stu-id="638b2-109">Most education software developers learn early on that class roster is one of the key pieces of information they need to run their application, and it's typically locked away inside a school Student Information System (SIS).</span></span> <span data-ttu-id="638b2-110">教師が新しいアプリケーションをクラスルームに導入しようとする場合、手動で名簿データをアプリケーションにインポートするために多くの時間を費やすことになります。</span><span class="sxs-lookup"><span data-stu-id="638b2-110">Any time teachers bring a new application into their classroom, they spend time manually importing roster data into the app.</span></span> <span data-ttu-id="638b2-111">多くの独立系ソフトウェア ベンダー (ISV) では、SIS に接続して名簿データをインポートすることによりこの問題に対処しています。</span><span class="sxs-lookup"><span data-stu-id="638b2-111">Many ISVs address this by connecting with a SIS to import roster data.</span></span> <span data-ttu-id="638b2-112">何百とある学生情報システムで、それぞれ独自の書式が使用されているということが課題となります。</span><span class="sxs-lookup"><span data-stu-id="638b2-112">With hundreds of Student Information Systems with proprietary formats, this can become a challenge.</span></span> <span data-ttu-id="638b2-113">[Microsoft School Data Sync](https://sds.microsoft.com/) と名簿 API を組み合わせることにより、アプリケーション開発者と学校がこの課題に対処できます。</span><span class="sxs-lookup"><span data-stu-id="638b2-113">[Microsoft School Data Sync](https://sds.microsoft.com/), combined with roster APIs, addresses this challenge for application developers and schools.</span></span>

<span data-ttu-id="638b2-114">名簿 API で可能になるシナリオのいくつかを次に示します:</span><span class="sxs-lookup"><span data-stu-id="638b2-114">The following are some of the scenarios that the roster APIs enable:</span></span>

- [<span data-ttu-id="638b2-115">学校内の全クラスを取得する</span><span class="sxs-lookup"><span data-stu-id="638b2-115">Get all classes in a school</span></span>](/graph/api/educationschool-list-classes?view=graph-rest-1.0)
- [<span data-ttu-id="638b2-116">クラス内の全ユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="638b2-116">Get all users in a class</span></span>](/graph/api/educationclass-list-members?view=graph-rest-1.0)
- [<span data-ttu-id="638b2-117">教師の担当する全クラスを取得する</span><span class="sxs-lookup"><span data-stu-id="638b2-117">Get all the classes I teach</span></span>](/graph/api/educationuser-list-classes?view=graph-rest-1.0)


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a><span data-ttu-id="638b2-118">Microsoft Teams を使用して割り当てタブでクラス割り当てを作成する</span><span class="sxs-lookup"><span data-stu-id="638b2-118">Use Microsoft Teams to create class assignments in an assignments tab</span></span>


<span data-ttu-id="638b2-119">割り当て API を使用することにより、クラス割り当てを管理する Web アプリを作成し、新しいカスタム タブ上でアプリを Microsoft Teams に統合することができます。</span><span class="sxs-lookup"><span data-stu-id="638b2-119">You can use the assignments API to create a web app that manages class assignments and then integrate your app into Microsoft Teams on a new custom tab.</span></span>  

<span data-ttu-id="638b2-120">Office 365 の Microsoft Teams は、会話、コンテンツ、およびアプリを、クラスルールのための 1 つの場所にまとめるデジタル ハブです。</span><span class="sxs-lookup"><span data-stu-id="638b2-120">Microsoft Teams in Office 365 is a digital hub that brings conversations, content, and apps together in one place for classrooms.</span></span> <span data-ttu-id="638b2-121">Microsoft Teams は、タブ、コネクタ、およびボットの作成など、[豊富な機能拡張ポイントのセット](https://docs.microsoft.com/ja-JP/microsoftteams/platform/concepts/apps/apps-overview)を提供します。</span><span class="sxs-lookup"><span data-stu-id="638b2-121">Microsoft Teams provides a [rich set of extensibility points](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-overview), including creating Tabs, Connectors, and Bots.</span></span> <span data-ttu-id="638b2-122">それらの機能拡張ポイントでは、Microsoft Graph の教育機関向け API を呼び出すことにより、課題や提出を処理することができます。</span><span class="sxs-lookup"><span data-stu-id="638b2-122">These extensibility points can call education APIs in Microsoft Graph to work with assignments and submissions.</span></span> <span data-ttu-id="638b2-123">機能拡張ポイントを他の Microsoft Graph API や、課題と提出の API により有効にすることによって、さらに総合的なエクスペリエンスを構築します。</span><span class="sxs-lookup"><span data-stu-id="638b2-123">Build a more comprehensive experience by enabling your extension point with any other Microsoft Graph API along with assignment and submission APIs.</span></span>

<span data-ttu-id="638b2-124">教育機関向けに、教育機関のクラス (チーム) のコンテキストで Microsoft Teams カスタム タブが開かれており、作成や配布から、評価やフィードバックに至るまで、エンドツーエンドの割り当てフローを意味ある方法で管理できます。</span><span class="sxs-lookup"><span data-stu-id="638b2-124">For education, Microsoft Teams custom tab apps are opened in an education class (a team) context, where it makes sense to manage the end-to-end assignment flow, from creation and distribution to grading and feedback.</span></span> <span data-ttu-id="638b2-125">これは、Microsoft Teams で時間が節約され、日常的な作業が簡素化されることのほんの一例に過ぎません。この例の場合、教職員は雑務から解放されて学生に注意を集中できます。</span><span class="sxs-lookup"><span data-stu-id="638b2-125">This is just one example of how Microsoft Teams saves time and simplifies everyday logistics, leaving educators free to dedicate themselves to their students.</span></span>

<span data-ttu-id="638b2-126">次の図に、**理科 - 生物 1** のクラス用の課題カスタム タブで課題を管理するための Web アプリを示します。</span><span class="sxs-lookup"><span data-stu-id="638b2-126">The following image shows a web app for managing assignments in an Assignments custom Tab for a **Science - Biology 1** class.</span></span>

![理科 - 生物のクラス用 Microsoft Teams の課題タブのスクリーンショット](images/assignmentsinteams.png)


<span data-ttu-id="638b2-128">割り当て API により、Microsoft Teams 外でアプリが課題サービスと対話処理を実行できます。</span><span class="sxs-lookup"><span data-stu-id="638b2-128">With the assignment API, your app can interact with the assignment service outside of Microsoft Teams.</span></span> <span data-ttu-id="638b2-129">配布、期限、評価は Microsoft Teams によって処理される一方、システムには、学生のための機能豊富な学習エクスペリエンスが用意されています。</span><span class="sxs-lookup"><span data-stu-id="638b2-129">Microsoft Teams will handle distribution, due dates, and grading while your system can provide a rich learning experience to students.</span></span>
<span data-ttu-id="638b2-130">割り当て API によって有効になるシナリオ例のいくつかを次に示します:</span><span class="sxs-lookup"><span data-stu-id="638b2-130">The following are examples of a few scenarios enabled by the assignments API:</span></span>

- [<span data-ttu-id="638b2-131">アプリケーションにリンクした課題を追加する</span><span class="sxs-lookup"><span data-stu-id="638b2-131">Add an assignment that links to your application</span></span>](/graph/api/educationclass-post-assignments?view=graph-rest-beta) 
- [<span data-ttu-id="638b2-132">アプリケーションにリンクした課題について個々の学生に評価を割り当てる</span><span class="sxs-lookup"><span data-stu-id="638b2-132">Assign grades to individual students for assignments linked to your application</span></span>](/graph/api/educationsubmission-update?view=graph-rest-beta)
- [<span data-ttu-id="638b2-133">割り当てとその期限を示す学生ダッシュボードを作成する</span><span class="sxs-lookup"><span data-stu-id="638b2-133">Create a student dashboard to show which assignments are due by when</span></span>](/graph/api/educationclass-list-assignments?view=graph-rest-beta)


### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a><span data-ttu-id="638b2-134">学校管理者が、学校データ同期管理 (プレビュー) を使用して ID および名簿の同期を管理できるようにする</span><span class="sxs-lookup"><span data-stu-id="638b2-134">Enable school admins to manage identity and roster sync using School Data Sync Management (preview)</span></span>

<span data-ttu-id="638b2-135">[学校データ同期](https://sds.microsoft.com/)は、Azure Active Directory (Azure AD) および Office 365 により、学生の ID と名簿データを学生情報システムからインポートし、同期するプロセスを自動化するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="638b2-135">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing student identity and roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="638b2-136">情報が同期されると、名簿 API を使用することにより、名簿情報をアプリケーションに読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="638b2-136">When the information is synchronized, you can use the roster APIs to read the roster information into the applications.</span></span> <span data-ttu-id="638b2-137">学校の学生情報システムと学校データ同期との統合処理を担当するシステム統合担当者は、Microsoft Graph で [SDS 管理 API](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) を使用することにより、CSV ファイルまたはサポートされている SIS API コネクタのいずれかからの同期処理をセットアップすることができます。</span><span class="sxs-lookup"><span data-stu-id="638b2-137">If you're a system integrator setting up integration of a school's Student Information System with School Data Sync, you can use the [SDS management APIs](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta) in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="638b2-138">学校データ同期管理 API では、同期管理のためのエンドツーエンドのシナリオがサポートされています。たとえば:</span><span class="sxs-lookup"><span data-stu-id="638b2-138">School Data Sync management APIs support end-to-end scenarios for managing sync; for example:</span></span>

- [<span data-ttu-id="638b2-139">自動的に同期を開始する同期ファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="638b2-139">Create a synchronization profile that automatically starts a sync</span></span>](/graph/api/educationsynchronizationprofile-post?view=graph-rest-beta)
- <span data-ttu-id="638b2-140">[一時停止](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta)、[再開](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta)、および[リセット](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta)の操作により同期ライフサイクルを管理する</span><span class="sxs-lookup"><span data-stu-id="638b2-140">Manage sync lifecycle with [pause](/graph/api/educationsynchronizationprofile-pause?view=graph-rest-beta), [resume](/graph/api/educationsynchronizationprofile-resume?view=graph-rest-beta) and [reset](/graph/api/educationsynchronizationprofile-reset?view=graph-rest-beta) operations</span></span>

## <a name="api-reference"></a><span data-ttu-id="638b2-141">API リファレンス</span><span class="sxs-lookup"><span data-stu-id="638b2-141">API reference</span></span>
<span data-ttu-id="638b2-142">このサービスの API リファレンスをお探しですか?</span><span class="sxs-lookup"><span data-stu-id="638b2-142">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="638b2-143">Microsoft Graph v1.0 の Education API</span><span class="sxs-lookup"><span data-stu-id="638b2-143">Education API in Microsoft Graph v1.0</span></span>](/graph/api/resources/education-overview?view=graph-rest-1.0)
- [<span data-ttu-id="638b2-144">Microsoft Graph ベータ版の Education API</span><span class="sxs-lookup"><span data-stu-id="638b2-144">Education API in Microsoft Graph beta</span></span>](/graph/api/resources/education-overview?view=graph-rest-beta)


## <a name="next-steps"></a><span data-ttu-id="638b2-145">次のステップ</span><span class="sxs-lookup"><span data-stu-id="638b2-145">Next Steps</span></span>

- <span data-ttu-id="638b2-146">教育機関向け API を初めて使用する場合は、以下を参照してください:</span><span class="sxs-lookup"><span data-stu-id="638b2-146">To start using the education APIs, see:</span></span>
  - [<span data-ttu-id="638b2-147">名簿 API を使用する</span><span class="sxs-lookup"><span data-stu-id="638b2-147">Use the roster APIs</span></span>](/graph/api/resources/education-overview?view=graph-rest-1.0)
  - [<span data-ttu-id="638b2-148">割り当て API を使用する</span><span class="sxs-lookup"><span data-stu-id="638b2-148">Use the assignment APIs</span></span>](/graph/api/resources/educationassignment?view=graph-rest-beta)
  - [<span data-ttu-id="638b2-149">SDS 管理 API を使用する</span><span class="sxs-lookup"><span data-stu-id="638b2-149">Use the SDS management APIs</span></span>](/graph/api/resources/educationsynchronizationprofile?view=graph-rest-beta)
- <span data-ttu-id="638b2-150">[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) で教育機関向け API を試す。</span><span class="sxs-lookup"><span data-stu-id="638b2-150">Try the education APIs in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="638b2-151">次の教育関連サンプルについて調べる:</span><span class="sxs-lookup"><span data-stu-id="638b2-151">Explore the following education-related samples:</span></span>
  - [<span data-ttu-id="638b2-152">SSO および名簿管理についての .NET サンプル</span><span class="sxs-lookup"><span data-stu-id="638b2-152">.NET sample for SSO & Rostering</span></span>](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
  - [<span data-ttu-id="638b2-153">SSO および名簿管理についての Angular ノード サンプル</span><span class="sxs-lookup"><span data-stu-id="638b2-153">Angular Node sample for SSO & Rostering</span></span>](https://github.com/OfficeDev/O365-EDU-AngularNodeJS-Samples)   
  - [<span data-ttu-id="638b2-154">SSO および名簿管理についての Python サンプル</span><span class="sxs-lookup"><span data-stu-id="638b2-154">Python sample for SSO & Rostering</span></span>](https://github.com/OfficeDev/O365-EDU-Python-Samples)
  - [<span data-ttu-id="638b2-155">SSO および名簿管理についての PHP サンプル</span><span class="sxs-lookup"><span data-stu-id="638b2-155">PHP sample for for SSO & Rostering</span></span>](https://github.com/OfficeDev/O365-EDU-PHP-Samples)
  - [<span data-ttu-id="638b2-156">プロファイル管理 API のサンプル</span><span class="sxs-lookup"><span data-stu-id="638b2-156">Sample for profile management APIs</span></span>](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples) 



 

