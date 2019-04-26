---
title: Microsoft Graph での教育機関 API の操作
description: Microsoft Graph の教育機関 api は、学校、学生、教師、クラス、登録、割り当てなどの教育シナリオに関連する情報を使用して、Office 365 のリソースとデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b5dd443b9ccda48c586bc44f6f4e35523a5e000f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340667"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="1e296-104">Microsoft Graph での教育機関 API の操作</span><span class="sxs-lookup"><span data-stu-id="1e296-104">Working with education APIs in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e296-105">Microsoft Graph の教育機関 api は、学校、学生、教師、クラス、登録、割り当てなどの教育シナリオに関連する情報を使用して、Office 365 のリソースとデータを強化します。</span><span class="sxs-lookup"><span data-stu-id="1e296-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="1e296-106">これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。</span><span class="sxs-lookup"><span data-stu-id="1e296-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="1e296-107">教育機関 api には、Microsoft Teams の名簿および assignment サービスと対話するために使用できる名簿リソースと割り当てリソースが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e296-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="1e296-108">これらのリソースを使用して、学校の名簿を管理し、学生の課題を自動化することができます。</span><span class="sxs-lookup"><span data-stu-id="1e296-108">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="1e296-109">認証</span><span class="sxs-lookup"><span data-stu-id="1e296-109">Authorization</span></span>

<span data-ttu-id="1e296-110">Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e296-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="1e296-111">アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e296-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="1e296-112">また、アプリには適切なアクセス許可も必要です。</span><span class="sxs-lookup"><span data-stu-id="1e296-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="1e296-113">詳細については、「[教育機関アクセス許可](/graph/permissions-reference#education-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e296-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="1e296-114">学校の IT 管理者が同意できるようにする、アプリのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="1e296-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="1e296-115">Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e296-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="1e296-116">アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1e296-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="1e296-117">管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="1e296-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="1e296-118">同意ダイアログボックスをトリガーするには、次の REST 呼び出しを使用します。</span><span class="sxs-lookup"><span data-stu-id="1e296-118">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="1e296-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1e296-119">Parameter</span></span>|<span data-ttu-id="1e296-120">説明</span><span class="sxs-lookup"><span data-stu-id="1e296-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="1e296-121">テナント</span><span class="sxs-lookup"><span data-stu-id="1e296-121">Tenant</span></span>|<span data-ttu-id="1e296-122">学校のテナント ID です。</span><span class="sxs-lookup"><span data-stu-id="1e296-122">Tenant ID of the school.</span></span> <span data-ttu-id="1e296-123">onmicrosoft.com を含む、完全な ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="1e296-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="1e296-124">clientId</span><span class="sxs-lookup"><span data-stu-id="1e296-124">clientId</span></span>|<span data-ttu-id="1e296-125">アプリのクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="1e296-125">Client ID of the app.</span></span>|
|<span data-ttu-id="1e296-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="1e296-126">redirectUrl</span></span>|<span data-ttu-id="1e296-127">アプリのリダイレクト URL です。</span><span class="sxs-lookup"><span data-stu-id="1e296-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="1e296-128">名簿</span><span class="sxs-lookup"><span data-stu-id="1e296-128">Rostering</span></span>

<span data-ttu-id="1e296-129">名簿 API により、[Microsoft School Data Sync](https://sds.microsoft.com/) でプロビジョニングされた学校の Office 365 テナントからデータを抽出できます。これらの API により、学校、部署、教師、学生、名簿に関する情報にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1e296-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="1e296-130">API は、アプリのみの (同期) シナリオと、アプリ + ユーザー (対話型) シナリオの両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e296-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="1e296-131">対話型シナリオをサポートする API は、API を呼び出すユーザー ロールに基づく、領域に適した RBAC ポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="1e296-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="1e296-132">これにより、テナント内の管理構成に関わらず、一貫した API および最小のポリシー サーフェスが提供されます。</span><span class="sxs-lookup"><span data-stu-id="1e296-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="1e296-133">さらに、API は教育機関に特有のアクセス許可も提供し、適切なユーザーがデータに確実にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="1e296-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="1e296-134">名簿 API を使用すれば、アプリ ユーザーは次のことを把握できます。</span><span class="sxs-lookup"><span data-stu-id="1e296-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="1e296-135">自分が誰か</span><span class="sxs-lookup"><span data-stu-id="1e296-135">Who I am</span></span>
- <span data-ttu-id="1e296-136">自分が出席する、または教えるクラス</span><span class="sxs-lookup"><span data-stu-id="1e296-136">What classes I attend or teach</span></span>
- <span data-ttu-id="1e296-137">何を、いつまでにする必要があるか</span><span class="sxs-lookup"><span data-stu-id="1e296-137">What I need to do and by when</span></span>

<span data-ttu-id="1e296-138">名簿 API は、次の重要なリソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="1e296-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="1e296-139">[educationSchool](educationschool.md) - 学校を示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="1e296-140">[educationClass](educationclass.md) - 学校内のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="1e296-141">[educationTerm](educationterm.md) - 学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="1e296-142">[educationTeacher](educationteacher.md) - プライマリ ロールが 'Teacher' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="1e296-143">[educationStudent](educationstudent.md) - プライマリ ロールが 'student' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="1e296-144">名簿 API は次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e296-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="1e296-145">すべての学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e296-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="1e296-146">授業が実施されている学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e296-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="1e296-147">ユーザーの学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e296-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="1e296-148">すべてのクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-148">Get all classes</span></span>](../api/educationroot-list-classes.md )
- [<span data-ttu-id="1e296-149">学校内のクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="1e296-150">ユーザーのクラスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e296-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="1e296-151">学校にクラスを追加する</span><span class="sxs-lookup"><span data-stu-id="1e296-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="1e296-152">クラスの学生と教師を取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="1e296-153">クラスにメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="1e296-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="1e296-154">クラスの教師を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1e296-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="1e296-155">学校内のユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="1e296-156">課題</span><span class="sxs-lookup"><span data-stu-id="1e296-156">Assignments</span></span> 

<span data-ttu-id="1e296-157">割り当てに関連する教育機関 api を使用して、Microsoft Teams の割り当てと統合することができます。</span><span class="sxs-lookup"><span data-stu-id="1e296-157">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="1e296-158">教育機関向け office 365 の Microsoft Teams は同じ教育機関 api に基づいており、api を使用してできることについてのユースケースが提供されています。</span><span class="sxs-lookup"><span data-stu-id="1e296-158">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="1e296-159">アプリでは、これらの api を使用して、割り当てライフサイクルを通じて割り当てを操作できます。</span><span class="sxs-lookup"><span data-stu-id="1e296-159">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="1e296-160">割り当て api は、次の主要なリソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="1e296-160">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="1e296-161">[educationAssignment](educationassignment.md) -割り当て API のコアオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="1e296-161">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="1e296-162">学生またはチームのメンバーに割り当てられた、学習の一部としてクラス内の1つまたは複数の作業の単位を表します。</span><span class="sxs-lookup"><span data-stu-id="1e296-162">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="1e296-163">[educationSubmission](educationsubmission.md) -個人 (またはグループ) が割り当てに関して提出するリソース、およびその割り当てに関する関連する成績とフィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="1e296-163">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="1e296-164">[educationResource](educationresource.md) -割り当てまたは送信される learning オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="1e296-164">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="1e296-165">**educationResource**は、 **educationAssignment**または**educationSubmission**に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="1e296-165">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="1e296-166">割り当て api は、次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e296-166">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="1e296-167">割り当てを作成する</span><span class="sxs-lookup"><span data-stu-id="1e296-167">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="1e296-168">割り当てを発行する</span><span class="sxs-lookup"><span data-stu-id="1e296-168">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="1e296-169">割り当てリソースを作成する</span><span class="sxs-lookup"><span data-stu-id="1e296-169">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="1e296-170">送信リソースの作成</span><span class="sxs-lookup"><span data-stu-id="1e296-170">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="1e296-171">割り当ての送信</span><span class="sxs-lookup"><span data-stu-id="1e296-171">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="1e296-172">未送信割り当て</span><span class="sxs-lookup"><span data-stu-id="1e296-172">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="1e296-173">成績を取得し、学生にフィードバックを送る</span><span class="sxs-lookup"><span data-stu-id="1e296-173">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="1e296-174">割り当ての詳細を取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-174">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="1e296-175">割り当てに関連する教育機関 api の一般的なユースケースを次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-175">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="1e296-176">ユース ケース</span><span class="sxs-lookup"><span data-stu-id="1e296-176">Use case</span></span>|<span data-ttu-id="1e296-177">説明</span><span class="sxs-lookup"><span data-stu-id="1e296-177">Description</span></span>|<span data-ttu-id="1e296-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="1e296-178">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="1e296-179">割り当ての作成</span><span class="sxs-lookup"><span data-stu-id="1e296-179">Create assignments</span></span>|<span data-ttu-id="1e296-180">外部システムでは、クラスの割り当てを作成し、リソースを割り当てに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="1e296-180">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="1e296-181">割り当てを作成する</span><span class="sxs-lookup"><span data-stu-id="1e296-181">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="1e296-182">割り当て情報の読み取り</span><span class="sxs-lookup"><span data-stu-id="1e296-182">Read assignment information</span></span>|<span data-ttu-id="1e296-183">分析アプリケーションは、日付や成績など、割り当てと学生の送信に関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="1e296-183">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="1e296-184">割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-184">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="1e296-185">受講者の送信を追跡する</span><span class="sxs-lookup"><span data-stu-id="1e296-185">Track student submissions</span></span>|<span data-ttu-id="1e296-186">アプリは教師ダッシュボードを提供することができます。これは、学生からの、採点する必要がある送信の数を示します。</span><span class="sxs-lookup"><span data-stu-id="1e296-186">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="1e296-187">提出リソース</span><span class="sxs-lookup"><span data-stu-id="1e296-187">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="1e296-188">School data sync management</span><span class="sxs-lookup"><span data-stu-id="1e296-188">School data sync management</span></span>

<span data-ttu-id="1e296-189">[School data Sync](https://sds.microsoft.com/)は、azure Active Directory (azure AD) と Office 365 を使用して、学生情報システムから名簿データをインポートおよび同期するプロセスを自動化するのに便利です。</span><span class="sxs-lookup"><span data-stu-id="1e296-189">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="1e296-190">Microsoft Graph の school data sync 管理 api を使用して、CSV ファイルまたはサポートされている SIS API コネクタから同期をセットアップすることができます。</span><span class="sxs-lookup"><span data-stu-id="1e296-190">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="1e296-191">school data sync 管理 api は、次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="1e296-191">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="1e296-192">同期プロファイルの一覧表示</span><span class="sxs-lookup"><span data-stu-id="1e296-192">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="1e296-193">同期プロファイルを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-193">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="1e296-194">同期プロファイルの作成</span><span class="sxs-lookup"><span data-stu-id="1e296-194">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="1e296-195">同期プロファイルの削除</span><span class="sxs-lookup"><span data-stu-id="1e296-195">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="1e296-196">進行中の同期を一時停止する</span><span class="sxs-lookup"><span data-stu-id="1e296-196">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="1e296-197">一時停止した同期を再開する</span><span class="sxs-lookup"><span data-stu-id="1e296-197">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="1e296-198">同期をリセットする</span><span class="sxs-lookup"><span data-stu-id="1e296-198">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="1e296-199">アップロードしたファイルの同期を開始する</span><span class="sxs-lookup"><span data-stu-id="1e296-199">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="1e296-200">アップロード URL を取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-200">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="1e296-201">同期の状態を取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-201">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="1e296-202">同期エラーを取得する</span><span class="sxs-lookup"><span data-stu-id="1e296-202">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="1e296-203">次の手順</span><span class="sxs-lookup"><span data-stu-id="1e296-203">Next steps</span></span>
<span data-ttu-id="1e296-204">Microsoft Graph エデュケーション api を使用して、学生の課題と学校の名簿にアクセスする教育ソリューションを構築します。</span><span class="sxs-lookup"><span data-stu-id="1e296-204">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="1e296-205">詳細情報</span><span class="sxs-lookup"><span data-stu-id="1e296-205">To learn more:</span></span>

- <span data-ttu-id="1e296-206">自分のシナリオに最も役立つリソースと方法を検討する。</span><span class="sxs-lookup"><span data-stu-id="1e296-206">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="1e296-207">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。</span><span class="sxs-lookup"><span data-stu-id="1e296-207">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

