---
title: Microsoft Graph での教育機関 API の操作
description: Microsoft Graph の教育機関 API は、Office 365 のリソースとデータを、学校、学生、教師、クラス、入学を含む教育機関のシナリオと関連する情報によって強化します。 これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。
localization_priority: Priority
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 142c946ea71e734baf58521ae8c4e9b51d54405c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029345"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="c1969-104">Microsoft Graph での教育機関 API の操作</span><span class="sxs-lookup"><span data-stu-id="c1969-104">Working with education APIs in Microsoft Graph</span></span>

<span data-ttu-id="c1969-105">Microsoft Graph の教育機関 API は、Office 365 のリソースとデータを、学校、学生、教師、クラス、入学を含む教育機関のシナリオと関連する情報によって強化します。</span><span class="sxs-lookup"><span data-stu-id="c1969-105">The education APIs in Microsoft Graph enhance Office 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="c1969-106">これにより、教育関連のリソースと統合するソリューションのビルドが簡単になります。</span><span class="sxs-lookup"><span data-stu-id="c1969-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="c1969-107">教育機関 API には名簿リソースや割り当てリソースが含まれ、Microsoft Teams の名簿サービスとのやり取りに使用できます。</span><span class="sxs-lookup"><span data-stu-id="c1969-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams.</span></span> <span data-ttu-id="c1969-108">これらのリソースを使用して、学校の名簿を管理できます。</span><span class="sxs-lookup"><span data-stu-id="c1969-108">You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="c1969-109">認証</span><span class="sxs-lookup"><span data-stu-id="c1969-109">Authorization</span></span>

<span data-ttu-id="c1969-110">Microsoft Graph で教育機関 API を呼び出すために、アプリはアクセス トークンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1969-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="c1969-111">アクセス トークンの詳細については、「[Microsoft Graph を呼び出すためのトークンの取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1969-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="c1969-112">また、アプリには適切なアクセス許可も必要です。</span><span class="sxs-lookup"><span data-stu-id="c1969-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="c1969-113">詳細については、「[教育機関アクセス許可](/graph/permissions-reference#education-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1969-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span> 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="c1969-114">学校の IT 管理者が同意できるようにする、アプリのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="c1969-114">App permissions to enable school IT admins to consent</span></span> 

<span data-ttu-id="c1969-115">Microsoft Graph の教育機関 API と統合されたアプリを展開するには、まず学校の IT 管理者が、アプリが要求するアクセス許可に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1969-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="c1969-116">アクセス許可が変更にならない限り、この同意は一度だけ与えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="c1969-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="c1969-117">管理者が同意した後、アプリはテナント内のすべてのユーザーに対してプロビジョニングされます。</span><span class="sxs-lookup"><span data-stu-id="c1969-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="c1969-118">同意ダイアログ ボックスを表示するには、次の REST 呼び出しを使用します。</span><span class="sxs-lookup"><span data-stu-id="c1969-118">To show a consent dialog box, use the following REST call.</span></span>

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|<span data-ttu-id="c1969-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c1969-119">Parameter</span></span>|<span data-ttu-id="c1969-120">説明</span><span class="sxs-lookup"><span data-stu-id="c1969-120">Description</span></span>|
|:--------|:----------|
|<span data-ttu-id="c1969-121">テナント</span><span class="sxs-lookup"><span data-stu-id="c1969-121">Tenant</span></span>|<span data-ttu-id="c1969-122">学校のテナント ID です。</span><span class="sxs-lookup"><span data-stu-id="c1969-122">Tenant ID of the school.</span></span> <span data-ttu-id="c1969-123">onmicrosoft.com を含む、完全な ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="c1969-123">Use the full ID, which includes onmicrosoft.com.</span></span>|
|<span data-ttu-id="c1969-124">clientId</span><span class="sxs-lookup"><span data-stu-id="c1969-124">clientId</span></span>|<span data-ttu-id="c1969-125">アプリのクライアント ID です。</span><span class="sxs-lookup"><span data-stu-id="c1969-125">Client ID of the app.</span></span>|
|<span data-ttu-id="c1969-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="c1969-126">redirectUrl</span></span>|<span data-ttu-id="c1969-127">アプリのリダイレクト URL です。</span><span class="sxs-lookup"><span data-stu-id="c1969-127">App redirect URL.</span></span>|


## <a name="rostering"></a><span data-ttu-id="c1969-128">名簿</span><span class="sxs-lookup"><span data-stu-id="c1969-128">Rostering</span></span>

<span data-ttu-id="c1969-129">名簿 API により、[Microsoft School Data Sync](https://sds.microsoft.com/) でプロビジョニングされた学校の Office 365 テナントからデータを抽出できます。これらの API により、学校、部署、教師、学生、名簿に関する情報にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c1969-129">The rostering APIs enable you to extract data from a school's Office 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="c1969-130">API は、アプリのみの (同期) シナリオと、アプリ + ユーザー (対話型) シナリオの両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c1969-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="c1969-131">対話型シナリオをサポートする API は、API を呼び出すユーザー ロールに基づく、領域に適した RBAC ポリシーを適用します。</span><span class="sxs-lookup"><span data-stu-id="c1969-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="c1969-132">これにより、テナント内の管理構成に関わらず、一貫した API および最小のポリシー サーフェスが提供されます。</span><span class="sxs-lookup"><span data-stu-id="c1969-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="c1969-133">さらに、API は教育機関に特有のアクセス許可も提供し、適切なユーザーがデータに確実にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="c1969-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="c1969-134">名簿 API を使用すれば、アプリ ユーザーは次のことを把握できます。</span><span class="sxs-lookup"><span data-stu-id="c1969-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="c1969-135">自分が誰か</span><span class="sxs-lookup"><span data-stu-id="c1969-135">Who I am</span></span>
- <span data-ttu-id="c1969-136">自分が出席する、または教えるクラス</span><span class="sxs-lookup"><span data-stu-id="c1969-136">What classes I attend or teach</span></span>
- <span data-ttu-id="c1969-137">何を、いつまでにする必要があるか</span><span class="sxs-lookup"><span data-stu-id="c1969-137">What I need to do and by when</span></span>

<span data-ttu-id="c1969-138">名簿 API は、次の重要なリソースを提供します。</span><span class="sxs-lookup"><span data-stu-id="c1969-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="c1969-139">[educationSchool](educationschool.md) - 学校を示します。</span><span class="sxs-lookup"><span data-stu-id="c1969-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="c1969-140">[educationClass](educationclass.md) - 学校内のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="c1969-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="c1969-141">[educationTerm](educationterm.md) - 学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="c1969-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="c1969-142">[educationTeacher](educationteacher.md) - プライマリ ロールが 'Teacher' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="c1969-142">[educationTeacher](educationteacher.md) - Represents a users with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="c1969-143">[educationStudent](educationstudent.md) - プライマリ ロールが 'student' であるユーザーを示します。</span><span class="sxs-lookup"><span data-stu-id="c1969-143">[educationStudent](educationstudent.md) - Represents a users with the primary role of 'student'.</span></span>

<span data-ttu-id="c1969-144">名簿 API は次のシナリオをサポートします。</span><span class="sxs-lookup"><span data-stu-id="c1969-144">The rostering APIs support the following scenarios:</span></span>

- [<span data-ttu-id="c1969-145">すべての学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c1969-145">List all schools</span></span>](../api/educationroot-list-schools.md) 
- [<span data-ttu-id="c1969-146">授業が実施されている学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c1969-146">List schools in which a class is taught</span></span>](../api/educationclass-list-schools.md)
- [<span data-ttu-id="c1969-147">ユーザーの学校を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c1969-147">List schools for a user</span></span>](../api/educationuser-list-schools.md)
- [<span data-ttu-id="c1969-148">すべてのクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="c1969-148">Get all classes</span></span>](../api/educationroot-list-classes.md)
- [<span data-ttu-id="c1969-149">学校内のクラスを取得する</span><span class="sxs-lookup"><span data-stu-id="c1969-149">Get classes in a school</span></span>](../api/educationschool-list-classes.md)
- [<span data-ttu-id="c1969-150">ユーザーのクラスを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c1969-150">List classes for a user</span></span>](../api/educationuser-list-classes.md)
- [<span data-ttu-id="c1969-151">学校にクラスを追加する</span><span class="sxs-lookup"><span data-stu-id="c1969-151">Add classes to a school</span></span>](../api/educationschool-post-classes.md)
- [<span data-ttu-id="c1969-152">クラスの学生と教師を取得する</span><span class="sxs-lookup"><span data-stu-id="c1969-152">Get students and teachers for a class</span></span>](../api/educationclass-list-members.md)
- [<span data-ttu-id="c1969-153">クラスにメンバーを追加する</span><span class="sxs-lookup"><span data-stu-id="c1969-153">Add members to a class</span></span>](../api/educationclass-post-members.md) 
- [<span data-ttu-id="c1969-154">クラスの教師を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="c1969-154">List teachers for a class</span></span>](../api/educationclass-list-teachers.md)
- [<span data-ttu-id="c1969-155">学校内のユーザーを取得する</span><span class="sxs-lookup"><span data-stu-id="c1969-155">Get users in a school</span></span>](../api/educationschool-list-users.md)

<!-- Should you list delete scenarios here as well? -->

## <a name="next-steps"></a><span data-ttu-id="c1969-156">次の手順</span><span class="sxs-lookup"><span data-stu-id="c1969-156">Next steps</span></span>
<span data-ttu-id="c1969-157">Microsoft Graph 教育機関 API を使用して、学校の名簿にアクセスする教育機関向けソリューションをビルドする。</span><span class="sxs-lookup"><span data-stu-id="c1969-157">Use the Microsoft Graph education APIs to build education solutions that access school rosters.</span></span> <span data-ttu-id="c1969-158">詳細情報</span><span class="sxs-lookup"><span data-stu-id="c1969-158">To learn more:</span></span>

- <span data-ttu-id="c1969-159">自分のシナリオに最も役立つリソースと方法を検討する。</span><span class="sxs-lookup"><span data-stu-id="c1969-159">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="c1969-160">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API を試す。</span><span class="sxs-lookup"><span data-stu-id="c1969-160">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

