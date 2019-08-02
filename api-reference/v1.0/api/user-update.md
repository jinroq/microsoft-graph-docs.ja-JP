---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5fb7e0643c8caad977ab99d3dbb4d669c73d8d69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36026545"
---
# <a name="update-user"></a><span data-ttu-id="ec519-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="ec519-103">Update user</span></span>

<span data-ttu-id="ec519-104">ユーザー オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec519-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec519-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ec519-105">Permissions</span></span>
<span data-ttu-id="ec519-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec519-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec519-108">Permission type</span></span>      | <span data-ttu-id="ec519-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec519-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec519-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec519-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec519-111">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec519-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec519-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec519-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec519-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec519-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="ec519-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec519-114">Application</span></span> | <span data-ttu-id="ec519-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec519-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="ec519-116">**passwordProfile** プロパティを更新するときは、次のアクセス許可が必要です。Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="ec519-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="ec519-117">他のユーザーの**businessPhones**、**mobilePhone**、または**otherMails** のプロパティの更新を許可されているのは、管理者以外のユーザーまたは次のロールのいずれかを割り当てられたユーザーのみになります。ディレクトリ閲覧者、ゲスト招待元、メッセージ センター閲覧者およびレポート閲覧者。</span><span class="sxs-lookup"><span data-stu-id="ec519-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="ec519-118">詳細については、「[Azure AD で使用できるロール](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)」のヘルプデスク (パスワード) 管理者を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec519-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="ec519-119">User.ReadWrite.All または Directory.ReadWrite.All の委任またはアプリケーションのアクセス許可のいずれかが与えられているアプリの場合、これに該当します。</span><span class="sxs-lookup"><span data-stu-id="ec519-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="ec519-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec519-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="ec519-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec519-121">Request headers</span></span>
| <span data-ttu-id="ec519-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec519-122">Header</span></span>       | <span data-ttu-id="ec519-123">値</span><span class="sxs-lookup"><span data-stu-id="ec519-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ec519-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec519-124">Authorization</span></span>  | <span data-ttu-id="ec519-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ec519-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec519-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec519-127">Content-Type</span></span>  | <span data-ttu-id="ec519-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ec519-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec519-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec519-129">Request body</span></span>
<span data-ttu-id="ec519-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ec519-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ec519-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec519-133">Property</span></span>     | <span data-ttu-id="ec519-134">型</span><span class="sxs-lookup"><span data-stu-id="ec519-134">Type</span></span>   |<span data-ttu-id="ec519-135">説明</span><span class="sxs-lookup"><span data-stu-id="ec519-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec519-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="ec519-136">aboutMe</span></span>|<span data-ttu-id="ec519-137">String</span><span class="sxs-lookup"><span data-stu-id="ec519-137">String</span></span>|<span data-ttu-id="ec519-138">ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。</span><span class="sxs-lookup"><span data-stu-id="ec519-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="ec519-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ec519-139">accountEnabled</span></span>|<span data-ttu-id="ec519-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="ec519-140">Boolean</span></span>| <span data-ttu-id="ec519-141">アカウントが有効な場合は **true**。そうでない場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="ec519-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="ec519-142">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="ec519-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="ec519-143">birthday</span><span class="sxs-lookup"><span data-stu-id="ec519-143">birthday</span></span>|<span data-ttu-id="ec519-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec519-144">DateTimeOffset</span></span>|<span data-ttu-id="ec519-p106">ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ec519-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ec519-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="ec519-148">businessPhones</span></span>| <span data-ttu-id="ec519-149">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-149">String collection</span></span> | <span data-ttu-id="ec519-p107">ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="ec519-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="ec519-152">city</span><span class="sxs-lookup"><span data-stu-id="ec519-152">city</span></span>|<span data-ttu-id="ec519-153">String</span><span class="sxs-lookup"><span data-stu-id="ec519-153">String</span></span>|<span data-ttu-id="ec519-154">ユーザーがいる都市。</span><span class="sxs-lookup"><span data-stu-id="ec519-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="ec519-155">country</span><span class="sxs-lookup"><span data-stu-id="ec519-155">country</span></span>|<span data-ttu-id="ec519-156">String</span><span class="sxs-lookup"><span data-stu-id="ec519-156">String</span></span>|<span data-ttu-id="ec519-157">ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。</span><span class="sxs-lookup"><span data-stu-id="ec519-157">The country/region in which the user is located; for example, "US" or "UK".</span></span>|
|<span data-ttu-id="ec519-158">department</span><span class="sxs-lookup"><span data-stu-id="ec519-158">department</span></span>|<span data-ttu-id="ec519-159">String</span><span class="sxs-lookup"><span data-stu-id="ec519-159">String</span></span>|<span data-ttu-id="ec519-160">ユーザーが働いている部門の名前。</span><span class="sxs-lookup"><span data-stu-id="ec519-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="ec519-161">displayName</span><span class="sxs-lookup"><span data-stu-id="ec519-161">displayName</span></span>|<span data-ttu-id="ec519-162">String</span><span class="sxs-lookup"><span data-stu-id="ec519-162">String</span></span>|<span data-ttu-id="ec519-p108">アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ec519-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="ec519-167">givenName</span><span class="sxs-lookup"><span data-stu-id="ec519-167">givenName</span></span>|<span data-ttu-id="ec519-168">String</span><span class="sxs-lookup"><span data-stu-id="ec519-168">String</span></span>|<span data-ttu-id="ec519-169">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="ec519-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="ec519-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="ec519-170">hireDate</span></span>|<span data-ttu-id="ec519-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec519-171">DateTimeOffset</span></span>|<span data-ttu-id="ec519-p109">ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ec519-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ec519-175">interests</span><span class="sxs-lookup"><span data-stu-id="ec519-175">interests</span></span>|<span data-ttu-id="ec519-176">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-176">String collection</span></span>|<span data-ttu-id="ec519-177">ユーザーが自分の関心事を記述する一覧。</span><span class="sxs-lookup"><span data-stu-id="ec519-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="ec519-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="ec519-178">jobTitle</span></span>|<span data-ttu-id="ec519-179">String</span><span class="sxs-lookup"><span data-stu-id="ec519-179">String</span></span>|<span data-ttu-id="ec519-180">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="ec519-180">The user’s job title.</span></span>|
|<span data-ttu-id="ec519-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ec519-181">mailNickname</span></span>|<span data-ttu-id="ec519-182">String</span><span class="sxs-lookup"><span data-stu-id="ec519-182">String</span></span>|<span data-ttu-id="ec519-183">ユーザーの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="ec519-183">The mail alias for the user.</span></span> <span data-ttu-id="ec519-184">ユーザーの作成時に、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec519-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="ec519-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="ec519-185">mobilePhone</span></span>|<span data-ttu-id="ec519-186">String</span><span class="sxs-lookup"><span data-stu-id="ec519-186">String</span></span>|<span data-ttu-id="ec519-187">ユーザーの主な携帯電話の番号。</span><span class="sxs-lookup"><span data-stu-id="ec519-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="ec519-188">mySite</span><span class="sxs-lookup"><span data-stu-id="ec519-188">mySite</span></span>|<span data-ttu-id="ec519-189">String</span><span class="sxs-lookup"><span data-stu-id="ec519-189">String</span></span>|<span data-ttu-id="ec519-190">ユーザーの個人用サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="ec519-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="ec519-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="ec519-191">officeLocation</span></span>|<span data-ttu-id="ec519-192">String</span><span class="sxs-lookup"><span data-stu-id="ec519-192">String</span></span>|<span data-ttu-id="ec519-193">ユーザーの勤務先の場所。</span><span class="sxs-lookup"><span data-stu-id="ec519-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="ec519-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="ec519-194">onPremisesImmutableId</span></span>|<span data-ttu-id="ec519-195">String</span><span class="sxs-lookup"><span data-stu-id="ec519-195">String</span></span>|<span data-ttu-id="ec519-196">このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。</span><span class="sxs-lookup"><span data-stu-id="ec519-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="ec519-197">Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec519-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="ec519-198">**重要:** **$** と **_** の文字は、このプロパティを指定するときには使用できません。</span><span class="sxs-lookup"><span data-stu-id="ec519-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="ec519-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="ec519-199">otherMails</span></span>|<span data-ttu-id="ec519-200">String</span><span class="sxs-lookup"><span data-stu-id="ec519-200">String</span></span> |<span data-ttu-id="ec519-201">ユーザーの追加のメール アドレスの一覧 (例: `["bob@contoso.com", "Robert@fabrikam.com"]`)。</span><span class="sxs-lookup"><span data-stu-id="ec519-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="ec519-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="ec519-202">passwordPolicies</span></span>|<span data-ttu-id="ec519-203">String</span><span class="sxs-lookup"><span data-stu-id="ec519-203">String</span></span>|<span data-ttu-id="ec519-p112">ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"</span><span class="sxs-lookup"><span data-stu-id="ec519-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="ec519-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="ec519-208">passwordProfile</span></span>|[<span data-ttu-id="ec519-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="ec519-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="ec519-p113">ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="ec519-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="ec519-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="ec519-215">pastProjects</span></span>|<span data-ttu-id="ec519-216">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-216">String collection</span></span>|<span data-ttu-id="ec519-217">ユーザーが過去のプロジェクトを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="ec519-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="ec519-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="ec519-218">postalCode</span></span>|<span data-ttu-id="ec519-219">String</span><span class="sxs-lookup"><span data-stu-id="ec519-219">String</span></span>|<span data-ttu-id="ec519-p114">ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ec519-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="ec519-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="ec519-223">preferredLanguage</span></span>|<span data-ttu-id="ec519-224">String</span><span class="sxs-lookup"><span data-stu-id="ec519-224">String</span></span>|<span data-ttu-id="ec519-p115">ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。</span><span class="sxs-lookup"><span data-stu-id="ec519-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="ec519-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="ec519-227">responsibilities</span></span>|<span data-ttu-id="ec519-228">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-228">String collection</span></span>|<span data-ttu-id="ec519-229">ユーザーが自分の責任の範囲を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="ec519-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="ec519-230">schools</span><span class="sxs-lookup"><span data-stu-id="ec519-230">schools</span></span>|<span data-ttu-id="ec519-231">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-231">String collection</span></span>|<span data-ttu-id="ec519-232">ユーザーが在籍した学校を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="ec519-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="ec519-233">skills</span><span class="sxs-lookup"><span data-stu-id="ec519-233">skills</span></span>|<span data-ttu-id="ec519-234">String collection</span><span class="sxs-lookup"><span data-stu-id="ec519-234">String collection</span></span>|<span data-ttu-id="ec519-235">ユーザーが自分のスキルを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="ec519-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="ec519-236">state</span><span class="sxs-lookup"><span data-stu-id="ec519-236">state</span></span>|<span data-ttu-id="ec519-237">String</span><span class="sxs-lookup"><span data-stu-id="ec519-237">String</span></span>|<span data-ttu-id="ec519-238">ユーザーの住所の都道府県。</span><span class="sxs-lookup"><span data-stu-id="ec519-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="ec519-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="ec519-239">streetAddress</span></span>|<span data-ttu-id="ec519-240">String</span><span class="sxs-lookup"><span data-stu-id="ec519-240">String</span></span>|<span data-ttu-id="ec519-241">ユーザーの勤務先の番地。</span><span class="sxs-lookup"><span data-stu-id="ec519-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="ec519-242">surname</span><span class="sxs-lookup"><span data-stu-id="ec519-242">surname</span></span>|<span data-ttu-id="ec519-243">String</span><span class="sxs-lookup"><span data-stu-id="ec519-243">String</span></span>|<span data-ttu-id="ec519-244">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="ec519-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="ec519-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="ec519-245">usageLocation</span></span>|<span data-ttu-id="ec519-246">String</span><span class="sxs-lookup"><span data-stu-id="ec519-246">String</span></span>|<span data-ttu-id="ec519-247">2 文字の国コード (ISO 規格 3166)</span><span class="sxs-lookup"><span data-stu-id="ec519-247">A two-letter country code (ISO standard 3166).</span></span> <span data-ttu-id="ec519-248">国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。</span><span class="sxs-lookup"><span data-stu-id="ec519-248">Required for users who will be assigned licenses due to a legal requirement to check for availability of services in countries or regions.</span></span>  <span data-ttu-id="ec519-249">たとえば、"US"、"JP"、"GB" などです。</span><span class="sxs-lookup"><span data-stu-id="ec519-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="ec519-250">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="ec519-250">Not nullable.</span></span>|
|<span data-ttu-id="ec519-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec519-251">userPrincipalName</span></span>|<span data-ttu-id="ec519-252">String</span><span class="sxs-lookup"><span data-stu-id="ec519-252">String</span></span>|<span data-ttu-id="ec519-p117">ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](../resources/organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ec519-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="ec519-260">userType</span><span class="sxs-lookup"><span data-stu-id="ec519-260">userType</span></span>|<span data-ttu-id="ec519-261">String</span><span class="sxs-lookup"><span data-stu-id="ec519-261">String</span></span>|<span data-ttu-id="ec519-262">ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。</span><span class="sxs-lookup"><span data-stu-id="ec519-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="ec519-263">応答</span><span class="sxs-lookup"><span data-stu-id="ec519-263">Response</span></span>

<span data-ttu-id="ec519-264">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ec519-264">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="ec519-265">例</span><span class="sxs-lookup"><span data-stu-id="ec519-265">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec519-266">要求</span><span class="sxs-lookup"><span data-stu-id="ec519-266">Request</span></span>
<span data-ttu-id="ec519-267">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec519-267">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ec519-268">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec519-268">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec519-269">C#</span><span class="sxs-lookup"><span data-stu-id="ec519-269">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec519-270">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec519-270">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec519-271">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec519-271">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ec519-272">Java</span><span class="sxs-lookup"><span data-stu-id="ec519-272">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec519-273">応答</span><span class="sxs-lookup"><span data-stu-id="ec519-273">Response</span></span>
<span data-ttu-id="ec519-274">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ec519-274">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
