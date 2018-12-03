---
title: Microsoft Graph での教育機関 API の操作
description: 教育 graph Api では、Office 365 のリソースとは、学校、学生、教師、クラス、登録、および割り当てを含む、教育のシナリオに関連する情報を使用してデータを強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。
ms.openlocfilehash: 610a16af6993397ae9162fb27add97cd6c5af0ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073474"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="7360d-104">Microsoft Graph での教育機関 API の操作</span><span class="sxs-lookup"><span data-stu-id="7360d-104">Working with education APIs in Microsoft Graph</span></span>

> <span data-ttu-id="7360d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7360d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7360d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7360d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7360d-107">教育 graph Api では、Office 365 のリソースとは、学校、学生、教師、クラス、登録、および割り当てを含む、教育のシナリオに関連する情報を使用してデータを強化します。</span><span class="sxs-lookup"><span data-stu-id="7360d-107">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, enrollments, and assignments.</span></span> <span data-ttu-id="7360d-108">これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。</span><span class="sxs-lookup"><span data-stu-id="7360d-108">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="7360d-109">教育には rostering リソースおよびマイクロソフトのチームで rostering および割り当てのサービスと対話するのに使用できる割り当てリソースに Api が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7360d-109">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering and assignment services in Microsoft Teams.</span></span> <span data-ttu-id="7360d-110">学校名簿を管理し、受講生受講者の割り当てを自動化するのには、これらのリソースを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7360d-110">You can use these resources to manage a school roster and automate student assignments.</span></span>

## <a name="authorization"></a><span data-ttu-id="7360d-111">認証</span><span class="sxs-lookup"><span data-stu-id="7360d-111">Authorization</span></span>

<span data-ttu-id="7360d-112">Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7360d-112">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="7360d-113">アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7360d-113">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="7360d-114">また、アプリには適切なアクセス許可も必要です。</span><span class="sxs-lookup"><span data-stu-id="7360d-114">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="7360d-115">詳細については、「[教育機関アクセス許可](/graph/permissions-reference#education-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7360d-115">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="7360d-116">学校の IT 管理者が同意できるようにする、アプリのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="7360d-116">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="7360d-117">Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7360d-117">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="7360d-118">アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7360d-118">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="7360d-119">管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="7360d-119">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="7360d-120">同意ダイアログ ボックスをトリガーするには、次の REST 呼び出しを使用します。</span><span class="sxs-lookup"><span data-stu-id="7360d-120">To trigger a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="7360d-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7360d-121">Parameter</span></span>|<span data-ttu-id="7360d-122">説明</span><span class="sxs-lookup"><span data-stu-id="7360d-122">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="7360d-123">テナント</span><span class="sxs-lookup"><span data-stu-id="7360d-123">Tenant</span></span>|<span data-ttu-id="7360d-124">学校のテナント ID です。</span><span class="sxs-lookup"><span data-stu-id="7360d-124">Tenant ID of the school.</span></span> <span data-ttu-id="7360d-125">onmicrosoft.com を含む、完全な ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="7360d-125">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="7360d-126">clientId</span><span class="sxs-lookup"><span data-stu-id="7360d-126">clientId</span></span>|<span data-ttu-id="7360d-127">アプリのクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="7360d-127">Client ID of the app.</span></span>|
|<span data-ttu-id="7360d-128">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="7360d-128">redirectUrl</span></span>|<span data-ttu-id="7360d-129">アプリのリダイレクト URL です。</span><span class="sxs-lookup"><span data-stu-id="7360d-129">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="7360d-130">名簿</span><span class="sxs-lookup"><span data-stu-id="7360d-130">Rostering</span></span>

<span data-ttu-id="7360d-131">名簿 API により、[Microsoft School Data Sync](https://sds.microsoft.com/) でプロビジョニングされた学校の Office 365 テナントからデータを抽出できます。これらの API により、学校、部署、教師、学生、名簿に関する情報にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="7360d-131">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="7360d-132">API は、アプリのみの (同期) シナリオと、アプリ + ユーザー (対話型) シナリオの両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7360d-132">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="7360d-133">対話型シナリオをサポートする API は、API を呼び出すユーザー ロールに基づく、領域に適した RBAC ポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="7360d-133">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="7360d-134">これにより、テナント内の管理構成に関わらず、一貫した API および最小のポリシー サーフェスが提供されます。</span><span class="sxs-lookup"><span data-stu-id="7360d-134">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="7360d-135">さらに、API は教育機関に特有のアクセス許可も提供し、適切なユーザーがデータに確実にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="7360d-135">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="7360d-136">名簿 API を使用すれば、アプリ ユーザーは次のことを把握できます。</span><span class="sxs-lookup"><span data-stu-id="7360d-136">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="7360d-137">自分が誰か</span><span class="sxs-lookup"><span data-stu-id="7360d-137">Who I am</span></span>
- <span data-ttu-id="7360d-138">自分が出席する、または教えるクラス</span><span class="sxs-lookup"><span data-stu-id="7360d-138">What classes I attend or teach</span></span>
- <span data-ttu-id="7360d-139">何を、いつまでにする必要があるか</span><span class="sxs-lookup"><span data-stu-id="7360d-139">What I need to do and by when</span></span>

<span data-ttu-id="7360d-140">名簿 API は、次の重要なリソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="7360d-140">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="7360d-141">[educationSchool](educationschool.md) - 学校を示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-141">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="7360d-142">[educationClass](educationclass.md) - 学校内のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-142">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="7360d-143">[educationTerm](educationterm.md) - 学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-143">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="7360d-144">[educationTeacher](educationteacher.md) - プライマリ ロールが 'Teacher' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-144">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="7360d-145">[educationStudent](educationstudent.md) - プライマリ ロールが 'student' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-145">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="7360d-146">名簿 API は次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="7360d-146">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="7360d-147">すべての学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7360d-147">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="7360d-148">授業が実施されている学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7360d-148">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="7360d-149">ユーザーの学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7360d-149">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="7360d-150">すべてのクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="7360d-150">Get all classes</span></span>](../api/educationroot_list_classes.md )
- [<span data-ttu-id="7360d-151">学校内のクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="7360d-151">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="7360d-152">ユーザーのクラスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7360d-152">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="7360d-153">学校にクラスを追加する</span><span class="sxs-lookup"><span data-stu-id="7360d-153">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="7360d-154">クラスの学生と教師を取得する</span><span class="sxs-lookup"><span data-stu-id="7360d-154">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="7360d-155">クラスにメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="7360d-155">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="7360d-156">クラスの教師を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7360d-156">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="7360d-157">学校内のユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="7360d-157">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a><span data-ttu-id="7360d-158">割り当て</span><span class="sxs-lookup"><span data-stu-id="7360d-158">Assignments</span></span> 

<span data-ttu-id="7360d-159">割り当てに関連する教育の Api を使用するにはマイクロソフトのチームでの割り当てとを統合します。</span><span class="sxs-lookup"><span data-stu-id="7360d-159">You can use the assignment-related education APIs to integrate with assignments in Microsoft Teams.</span></span> <span data-ttu-id="7360d-160">教育を Office 365 で、マイクロソフトのチームでは、Api では、同じ教育に基づいており、ユース ケースでは、Api で行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7360d-160">Microsoft Teams in Office 365 for Education is based on the same education APIs, and provides a use case for what you can do with the APIs.</span></span> <span data-ttu-id="7360d-161">アプリでは、これらの Api を使用して、割り当てのライフ サイクル全体の割り当てと対話します。</span><span class="sxs-lookup"><span data-stu-id="7360d-161">Your app can use these APIs to interact with assignments throughout the assignment lifecycle.</span></span> 

<span data-ttu-id="7360d-162">割り当て Api は、次のキーのリソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="7360d-162">The assignment APIs provide the following key resources:</span></span>

- <span data-ttu-id="7360d-163">[educationAssignment](educationassignment.md) - 割り当て API の主要なオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7360d-163">[educationAssignment](educationassignment.md) - The core object of the assignments API.</span></span> <span data-ttu-id="7360d-164">タスクや、研究の一部として、クラスの受講生受講者またはチームのメンバーに割り当てられた作業時間の単位を表します。</span><span class="sxs-lookup"><span data-stu-id="7360d-164">Represents a task or unit of work assigned to a student or team member in a class as part of their study.</span></span>
- <span data-ttu-id="7360d-165">[educationSubmission](educationsubmission.md) ・ リソースを表しますが、個人 (またはグループ) は、割り当てと関連付けられているグレードとその割り当てのためのフィードバックを送信します。</span><span class="sxs-lookup"><span data-stu-id="7360d-165">[educationSubmission](educationsubmission.md) - Represents the resources that an individual (or group) submits for an assignment and the associated grade and feedback for that assignment.</span></span>
- <span data-ttu-id="7360d-166">[educationResource](educationresource.md) - 学習オブジェクトを表しますは、割り当てられている、送信されています。</span><span class="sxs-lookup"><span data-stu-id="7360d-166">[educationResource](educationresource.md) - Represents the learning object that is being assigned or submitted.</span></span> <span data-ttu-id="7360d-167">**EducationResource**では、 **educationAssignment**や、 **educationSubmission**に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="7360d-167">An **educationResource** is associated with an **educationAssignment** and/or an **educationSubmission**.</span></span>

<span data-ttu-id="7360d-168">割り当て Api では、次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="7360d-168">The assignment APIs support the following scenarios:</span></span>

- [<span data-ttu-id="7360d-169">割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="7360d-169">Create assignment</span></span>](../api/educationclass-post-assignments.md)
- [<span data-ttu-id="7360d-170">割り当てを発行します。</span><span class="sxs-lookup"><span data-stu-id="7360d-170">Publish assignment</span></span>](../api/educationassignment-publish.md)
- [<span data-ttu-id="7360d-171">割り当てリソースを作成します。</span><span class="sxs-lookup"><span data-stu-id="7360d-171">Create assignment resource</span></span>](../api/educationassignment-post-resources.md)
- [<span data-ttu-id="7360d-172">送信リソースを作成します。</span><span class="sxs-lookup"><span data-stu-id="7360d-172">Create submission resource</span></span>](../api/educationsubmission-post-resources.md)
- [<span data-ttu-id="7360d-173">割り当てを送信します。</span><span class="sxs-lookup"><span data-stu-id="7360d-173">Submit assignment</span></span>](../api/educationsubmission-submit.md) 
- [<span data-ttu-id="7360d-174">割り当てを unsubmit します。</span><span class="sxs-lookup"><span data-stu-id="7360d-174">Unsubmit assignment</span></span>](../api/educationsubmission-unsubmit.md)   
- [<span data-ttu-id="7360d-175">受講者の成績とフィードバックを返す</span><span class="sxs-lookup"><span data-stu-id="7360d-175">Return grades and feedback to student</span></span>](../api/educationsubmission-return.md) 
- [<span data-ttu-id="7360d-176">割り当ての詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="7360d-176">Get assignment details</span></span>](../api/educationuser-list-assignments.md)

<span data-ttu-id="7360d-177">割り当てに関連する教育の Api のいくつかの一般的な使用例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7360d-177">The following are some common use cases for the assignment-related education APIs.</span></span>

|<span data-ttu-id="7360d-178">使用例</span><span class="sxs-lookup"><span data-stu-id="7360d-178">Use case</span></span>|<span data-ttu-id="7360d-179">説明</span><span class="sxs-lookup"><span data-stu-id="7360d-179">Description</span></span>|<span data-ttu-id="7360d-180">関連項目</span><span class="sxs-lookup"><span data-stu-id="7360d-180">See also</span></span>|
|:-------|:----------|:-------|
|<span data-ttu-id="7360d-181">割り当てを作成します</span><span class="sxs-lookup"><span data-stu-id="7360d-181">Create assignments</span></span>|<span data-ttu-id="7360d-182">外部システムでは、クラスの割り当てを作成でき、割り当てのリソースに接続することができます。</span><span class="sxs-lookup"><span data-stu-id="7360d-182">An external system can create an assignment for the class and attach resources to the assignment.</span></span>|[<span data-ttu-id="7360d-183">割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="7360d-183">Create assignment</span></span>](../api/educationassignment-post-resources.md)|
|<span data-ttu-id="7360d-184">割り当て情報を読み取る</span><span class="sxs-lookup"><span data-stu-id="7360d-184">Read assignment information</span></span>|<span data-ttu-id="7360d-185">分析アプリケーションでは、割り当てと、受講生受講者の提出書類、日付や成績などに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="7360d-185">An analytics application can get information about assignments and student submissions, including dates and grades.</span></span>|[<span data-ttu-id="7360d-186">割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="7360d-186">Get assignment</span></span>](../api/educationassignment-get.md)|
|<span data-ttu-id="7360d-187">受講者の提出書類を追跡します。</span><span class="sxs-lookup"><span data-stu-id="7360d-187">Track student submissions</span></span>|<span data-ttu-id="7360d-188">先生のダッシュ ボードに焼き付けることが必要な受講者からの提出書類の数を表示するアプリを提供します。</span><span class="sxs-lookup"><span data-stu-id="7360d-188">Your app can provide a teacher dashboard that shows how many submissions from students need to be graded.</span></span>|[<span data-ttu-id="7360d-189">送信リソース</span><span class="sxs-lookup"><span data-stu-id="7360d-189">Submission resource</span></span>](educationsubmission.md)|

## <a name="school-data-sync-management"></a><span data-ttu-id="7360d-190">学校のデータの同期の管理</span><span class="sxs-lookup"><span data-stu-id="7360d-190">School data sync management</span></span>

<span data-ttu-id="7360d-191">[学校のデータの同期](https://sds.microsoft.com/)は、インポートして、Azure Active Directory (AD の Azure) と Office 365 の学生情報システムからの名簿データの同期のプロセスを自動化するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="7360d-191">[School Data Sync](https://sds.microsoft.com/) helps to automate the process of importing and synchronizing roster data from student information systems with Azure Active Directory (Azure AD) and Office 365.</span></span> <span data-ttu-id="7360d-192">CSV ファイルまたはサポートされている API の SIS のコネクタのいずれかから同期を設定するのには、Microsoft Graph で学校のデータの同期管理の Api を使用できます。</span><span class="sxs-lookup"><span data-stu-id="7360d-192">You can use the school data sync management APIs in Microsoft Graph to set up synchronization from either a CSV file or a supported SIS API connector.</span></span>

<span data-ttu-id="7360d-193">学校のデータは、管理 Api のサポートを次のシナリオを同期させます。</span><span class="sxs-lookup"><span data-stu-id="7360d-193">The school data sync management APIs support the following scenarios:</span></span>

- [<span data-ttu-id="7360d-194">同期プロファイルのリスト</span><span class="sxs-lookup"><span data-stu-id="7360d-194">List synchronization profiles</span></span>](../api/educationsynchronizationprofile-list.md)
- [<span data-ttu-id="7360d-195">同期プロファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="7360d-195">Get synchronization profile</span></span>](../api/educationsynchronizationprofile-get.md)
- [<span data-ttu-id="7360d-196">同期プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="7360d-196">Create synchronization profile</span></span>](../api/educationsynchronizationprofile-post.md)
- [<span data-ttu-id="7360d-197">同期プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="7360d-197">Delete synchronization profile</span></span>](../api/educationsynchronizationprofile-delete.md)
- [<span data-ttu-id="7360d-198">進行中の同期を一時停止します。</span><span class="sxs-lookup"><span data-stu-id="7360d-198">Pause an ongoing sync</span></span>](../api/educationsynchronizationprofile-pause.md)
- [<span data-ttu-id="7360d-199">一時停止中の同期を再開します。</span><span class="sxs-lookup"><span data-stu-id="7360d-199">Resume a paused sync</span></span>](../api/educationsynchronizationprofile-resume.md)
- [<span data-ttu-id="7360d-200">同期をリセットします。</span><span class="sxs-lookup"><span data-stu-id="7360d-200">Reset a sync</span></span>](../api/educationsynchronizationprofile-reset.md)
- [<span data-ttu-id="7360d-201">アップロードされたファイルの同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="7360d-201">Start sync for uploaded files</span></span>](../api/educationsynchronizationprofile-start.md) 
- [<span data-ttu-id="7360d-202">アップロード先の URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="7360d-202">Get an upload URL</span></span>](../api/educationsynchronizationprofile-uploadurl.md)
- [<span data-ttu-id="7360d-203">同期のステータスを取得します。</span><span class="sxs-lookup"><span data-stu-id="7360d-203">Get status of a sync</span></span>](../api/educationsynchronizationprofilestatus-get.md)
- [<span data-ttu-id="7360d-204">同期エラーが発生をします。</span><span class="sxs-lookup"><span data-stu-id="7360d-204">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a><span data-ttu-id="7360d-205">次の手順</span><span class="sxs-lookup"><span data-stu-id="7360d-205">Next steps</span></span>
<span data-ttu-id="7360d-206">Graph 教育 Api を使用すると、受講生受講者の割り当てと、学校の名簿にアクセスするための教育ソリューションを構築できます。</span><span class="sxs-lookup"><span data-stu-id="7360d-206">Use the Microsoft Graph education APIs to build education solutions that access student assignments and school rosters.</span></span> <span data-ttu-id="7360d-207">詳細情報</span><span class="sxs-lookup"><span data-stu-id="7360d-207">To learn more:</span></span>

- <span data-ttu-id="7360d-208">自分のシナリオに最も役立つリソースと方法を検討する。</span><span class="sxs-lookup"><span data-stu-id="7360d-208">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="7360d-209">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。</span><span class="sxs-lookup"><span data-stu-id="7360d-209">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

