---
title: ユーザーを更新する
description: ユーザー オブジェクトのプロパティを更新します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af8d2c99d814c8a7b82e905e3fbbc7d5709bb9d6
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396857"
---
# <a name="update-user"></a><span data-ttu-id="7271e-103">ユーザーを更新する</span><span class="sxs-lookup"><span data-stu-id="7271e-103">Update user</span></span>

<span data-ttu-id="7271e-104">ユーザー オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7271e-104">Update the properties of a user object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7271e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7271e-105">Permissions</span></span>
<span data-ttu-id="7271e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7271e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7271e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7271e-108">Permission type</span></span>      | <span data-ttu-id="7271e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7271e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7271e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7271e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7271e-111">User.ReadWrite、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7271e-111">User.ReadWrite, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7271e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7271e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7271e-113">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7271e-113">User.ReadWrite</span></span>    |
|<span data-ttu-id="7271e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7271e-114">Application</span></span> | <span data-ttu-id="7271e-115">User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7271e-115">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

>[!NOTE]
> - <span data-ttu-id="7271e-116">**passwordProfile** プロパティを更新するときは、次のアクセス許可が必要です。Directory.AccessAsUser.All。</span><span class="sxs-lookup"><span data-stu-id="7271e-116">When updating the passwordProfile property, the following permission is required: Directory.AccessAsUser.All.</span></span>
> - <span data-ttu-id="7271e-117">他のユーザーの**businessPhones**、**mobilePhone**、または**otherMails** のプロパティの更新を許可されているのは、管理者以外のユーザーまたは次のロールのいずれかを割り当てられたユーザーのみになります。ディレクトリ閲覧者、ゲスト招待元、メッセージ センター閲覧者およびレポート閲覧者。</span><span class="sxs-lookup"><span data-stu-id="7271e-117">Updating another user's **businessPhones**, **mobilePhone**, or **otherMails** property is only allowed on users who are non-administrators or assigned one of the following roles: Directory Readers, Guest Inviter, Message Center Reader, and Reports Reader.</span></span> <span data-ttu-id="7271e-118">詳細については、「[Azure AD で使用できるロール](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)」のヘルプデスク (パスワード) 管理者を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7271e-118">For more details, see Helpdesk (Password) Administrator in [Azure AD available roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).</span></span>  <span data-ttu-id="7271e-119">User.ReadWrite.All または Directory.ReadWrite.All の委任またはアプリケーションのアクセス許可のいずれかが与えられているアプリの場合、これに該当します。</span><span class="sxs-lookup"><span data-stu-id="7271e-119">This is the case for apps granted either the User.ReadWrite.All or Directory.ReadWrite.All delegated or application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="7271e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7271e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="7271e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7271e-121">Request headers</span></span>
| <span data-ttu-id="7271e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7271e-122">Header</span></span>       | <span data-ttu-id="7271e-123">値</span><span class="sxs-lookup"><span data-stu-id="7271e-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="7271e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7271e-124">Authorization</span></span>  | <span data-ttu-id="7271e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7271e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7271e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7271e-127">Content-Type</span></span>  | <span data-ttu-id="7271e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7271e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7271e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="7271e-129">Request body</span></span>
<span data-ttu-id="7271e-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7271e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7271e-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7271e-133">Property</span></span>     | <span data-ttu-id="7271e-134">型</span><span class="sxs-lookup"><span data-stu-id="7271e-134">Type</span></span>   |<span data-ttu-id="7271e-135">説明</span><span class="sxs-lookup"><span data-stu-id="7271e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7271e-136">aboutMe</span><span class="sxs-lookup"><span data-stu-id="7271e-136">aboutMe</span></span>|<span data-ttu-id="7271e-137">String</span><span class="sxs-lookup"><span data-stu-id="7271e-137">String</span></span>|<span data-ttu-id="7271e-138">ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。</span><span class="sxs-lookup"><span data-stu-id="7271e-138">A freeform text entry field for the user to describe themselves.</span></span>|
|<span data-ttu-id="7271e-139">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="7271e-139">accountEnabled</span></span>|<span data-ttu-id="7271e-140">ブール値</span><span class="sxs-lookup"><span data-stu-id="7271e-140">Boolean</span></span>| <span data-ttu-id="7271e-141">アカウントが有効な場合は **true**。そうでない場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="7271e-141">**true** if the account is enabled; otherwise, **false**.</span></span> <span data-ttu-id="7271e-142">このプロパティは、ユーザーの作成時に必要です。</span><span class="sxs-lookup"><span data-stu-id="7271e-142">This property is required when a user is created.</span></span>    |
|<span data-ttu-id="7271e-143">birthday</span><span class="sxs-lookup"><span data-stu-id="7271e-143">birthday</span></span>|<span data-ttu-id="7271e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7271e-144">DateTimeOffset</span></span>|<span data-ttu-id="7271e-p106">ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7271e-p106">The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7271e-148">businessPhones</span><span class="sxs-lookup"><span data-stu-id="7271e-148">businessPhones</span></span>| <span data-ttu-id="7271e-149">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-149">String collection</span></span> | <span data-ttu-id="7271e-p107">ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。</span><span class="sxs-lookup"><span data-stu-id="7271e-p107">The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.</span></span>|
|<span data-ttu-id="7271e-152">city</span><span class="sxs-lookup"><span data-stu-id="7271e-152">city</span></span>|<span data-ttu-id="7271e-153">String</span><span class="sxs-lookup"><span data-stu-id="7271e-153">String</span></span>|<span data-ttu-id="7271e-154">ユーザーがいる都市。</span><span class="sxs-lookup"><span data-stu-id="7271e-154">The city in which the user is located.</span></span>|
|<span data-ttu-id="7271e-155">country</span><span class="sxs-lookup"><span data-stu-id="7271e-155">country</span></span>|<span data-ttu-id="7271e-156">String</span><span class="sxs-lookup"><span data-stu-id="7271e-156">String</span></span>|<span data-ttu-id="7271e-157">ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。</span><span class="sxs-lookup"><span data-stu-id="7271e-157">The country/region in which the user is located; for example, "US" or "UK".</span></span>|
|<span data-ttu-id="7271e-158">department</span><span class="sxs-lookup"><span data-stu-id="7271e-158">department</span></span>|<span data-ttu-id="7271e-159">String</span><span class="sxs-lookup"><span data-stu-id="7271e-159">String</span></span>|<span data-ttu-id="7271e-160">ユーザーが働いている部門の名前。</span><span class="sxs-lookup"><span data-stu-id="7271e-160">The name for the department in which the user works.</span></span>|
|<span data-ttu-id="7271e-161">displayName</span><span class="sxs-lookup"><span data-stu-id="7271e-161">displayName</span></span>|<span data-ttu-id="7271e-162">String</span><span class="sxs-lookup"><span data-stu-id="7271e-162">String</span></span>|<span data-ttu-id="7271e-p108">アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7271e-p108">The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="7271e-167">givenName</span><span class="sxs-lookup"><span data-stu-id="7271e-167">givenName</span></span>|<span data-ttu-id="7271e-168">String</span><span class="sxs-lookup"><span data-stu-id="7271e-168">String</span></span>|<span data-ttu-id="7271e-169">ユーザーの名。</span><span class="sxs-lookup"><span data-stu-id="7271e-169">The given name (first name) of the user.</span></span>|
|<span data-ttu-id="7271e-170">hireDate</span><span class="sxs-lookup"><span data-stu-id="7271e-170">hireDate</span></span>|<span data-ttu-id="7271e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7271e-171">DateTimeOffset</span></span>|<span data-ttu-id="7271e-p109">ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7271e-p109">The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7271e-175">interests</span><span class="sxs-lookup"><span data-stu-id="7271e-175">interests</span></span>|<span data-ttu-id="7271e-176">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-176">String collection</span></span>|<span data-ttu-id="7271e-177">ユーザーが自分の関心事を記述する一覧。</span><span class="sxs-lookup"><span data-stu-id="7271e-177">A list for the user to describe their interests.</span></span>|
|<span data-ttu-id="7271e-178">jobTitle</span><span class="sxs-lookup"><span data-stu-id="7271e-178">jobTitle</span></span>|<span data-ttu-id="7271e-179">String</span><span class="sxs-lookup"><span data-stu-id="7271e-179">String</span></span>|<span data-ttu-id="7271e-180">ユーザーの役職。</span><span class="sxs-lookup"><span data-stu-id="7271e-180">The user’s job title.</span></span>|
|<span data-ttu-id="7271e-181">mailNickname</span><span class="sxs-lookup"><span data-stu-id="7271e-181">mailNickname</span></span>|<span data-ttu-id="7271e-182">String</span><span class="sxs-lookup"><span data-stu-id="7271e-182">String</span></span>|<span data-ttu-id="7271e-183">ユーザーの電子メール エイリアス。</span><span class="sxs-lookup"><span data-stu-id="7271e-183">The mail alias for the user.</span></span> <span data-ttu-id="7271e-184">ユーザーの作成時に、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7271e-184">This property must be specified when a user is created.</span></span>|
|<span data-ttu-id="7271e-185">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="7271e-185">mobilePhone</span></span>|<span data-ttu-id="7271e-186">String</span><span class="sxs-lookup"><span data-stu-id="7271e-186">String</span></span>|<span data-ttu-id="7271e-187">ユーザーの主な携帯電話の番号。</span><span class="sxs-lookup"><span data-stu-id="7271e-187">The primary cellular telephone number for the user.</span></span>|
|<span data-ttu-id="7271e-188">mySite</span><span class="sxs-lookup"><span data-stu-id="7271e-188">mySite</span></span>|<span data-ttu-id="7271e-189">String</span><span class="sxs-lookup"><span data-stu-id="7271e-189">String</span></span>|<span data-ttu-id="7271e-190">ユーザーの個人用サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="7271e-190">The URL for the user's personal site.</span></span>|
|<span data-ttu-id="7271e-191">officeLocation</span><span class="sxs-lookup"><span data-stu-id="7271e-191">officeLocation</span></span>|<span data-ttu-id="7271e-192">String</span><span class="sxs-lookup"><span data-stu-id="7271e-192">String</span></span>|<span data-ttu-id="7271e-193">ユーザーの勤務先の場所。</span><span class="sxs-lookup"><span data-stu-id="7271e-193">The office location in the user's place of business.</span></span>|
|<span data-ttu-id="7271e-194">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="7271e-194">onPremisesImmutableId</span></span>|<span data-ttu-id="7271e-195">String</span><span class="sxs-lookup"><span data-stu-id="7271e-195">String</span></span>|<span data-ttu-id="7271e-196">このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。</span><span class="sxs-lookup"><span data-stu-id="7271e-196">This property is used to associate an on-premises Active Directory user account to their Azure AD user object.</span></span> <span data-ttu-id="7271e-197">Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7271e-197">This property must be specified when creating a new user account in the Graph if you are using a federated domain for the user’s **userPrincipalName** (UPN) property.</span></span> <span data-ttu-id="7271e-198">**重要:** **$** と **_** の文字は、このプロパティを指定するときには使用できません。</span><span class="sxs-lookup"><span data-stu-id="7271e-198">**Important:** The **$** and **_** characters cannot be used when specifying this property.</span></span>                            |
|<span data-ttu-id="7271e-199">otherMails</span><span class="sxs-lookup"><span data-stu-id="7271e-199">otherMails</span></span>|<span data-ttu-id="7271e-200">String</span><span class="sxs-lookup"><span data-stu-id="7271e-200">String</span></span> |<span data-ttu-id="7271e-201">ユーザーの追加のメール アドレスの一覧 (例: `["bob@contoso.com", "Robert@fabrikam.com"]`)。</span><span class="sxs-lookup"><span data-stu-id="7271e-201">A list of additional email addresses for the user; for example: `["bob@contoso.com", "Robert@fabrikam.com"]`.</span></span>|
|<span data-ttu-id="7271e-202">passwordPolicies</span><span class="sxs-lookup"><span data-stu-id="7271e-202">passwordPolicies</span></span>|<span data-ttu-id="7271e-203">String</span><span class="sxs-lookup"><span data-stu-id="7271e-203">String</span></span>|<span data-ttu-id="7271e-p112">ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"</span><span class="sxs-lookup"><span data-stu-id="7271e-p112">Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".</span></span>|
|<span data-ttu-id="7271e-208">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="7271e-208">passwordProfile</span></span>|[<span data-ttu-id="7271e-209">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="7271e-209">PasswordProfile</span></span>](../resources/passwordprofile.md)|<span data-ttu-id="7271e-p113">ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="7271e-p113">Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.</span></span>|
|<span data-ttu-id="7271e-215">pastProjects</span><span class="sxs-lookup"><span data-stu-id="7271e-215">pastProjects</span></span>|<span data-ttu-id="7271e-216">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-216">String collection</span></span>|<span data-ttu-id="7271e-217">ユーザーが過去のプロジェクトを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="7271e-217">A list for the user to enumerate their past projects.</span></span>|
|<span data-ttu-id="7271e-218">postalCode</span><span class="sxs-lookup"><span data-stu-id="7271e-218">postalCode</span></span>|<span data-ttu-id="7271e-219">String</span><span class="sxs-lookup"><span data-stu-id="7271e-219">String</span></span>|<span data-ttu-id="7271e-p114">ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7271e-p114">The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.</span></span>|
|<span data-ttu-id="7271e-223">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="7271e-223">preferredLanguage</span></span>|<span data-ttu-id="7271e-224">String</span><span class="sxs-lookup"><span data-stu-id="7271e-224">String</span></span>|<span data-ttu-id="7271e-p115">ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。</span><span class="sxs-lookup"><span data-stu-id="7271e-p115">The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".</span></span>|
|<span data-ttu-id="7271e-227">responsibilities</span><span class="sxs-lookup"><span data-stu-id="7271e-227">responsibilities</span></span>|<span data-ttu-id="7271e-228">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-228">String collection</span></span>|<span data-ttu-id="7271e-229">ユーザーが自分の責任の範囲を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="7271e-229">A list for the user to enumerate their responsibilities.</span></span>|
|<span data-ttu-id="7271e-230">schools</span><span class="sxs-lookup"><span data-stu-id="7271e-230">schools</span></span>|<span data-ttu-id="7271e-231">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-231">String collection</span></span>|<span data-ttu-id="7271e-232">ユーザーが在籍した学校を列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="7271e-232">A list for the user to enumerate the schools they have attended.</span></span>|
|<span data-ttu-id="7271e-233">skills</span><span class="sxs-lookup"><span data-stu-id="7271e-233">skills</span></span>|<span data-ttu-id="7271e-234">String collection</span><span class="sxs-lookup"><span data-stu-id="7271e-234">String collection</span></span>|<span data-ttu-id="7271e-235">ユーザーが自分のスキルを列挙する一覧。</span><span class="sxs-lookup"><span data-stu-id="7271e-235">A list for the user to enumerate their skills.</span></span>|
|<span data-ttu-id="7271e-236">state</span><span class="sxs-lookup"><span data-stu-id="7271e-236">state</span></span>|<span data-ttu-id="7271e-237">String</span><span class="sxs-lookup"><span data-stu-id="7271e-237">String</span></span>|<span data-ttu-id="7271e-238">ユーザーの住所の都道府県。</span><span class="sxs-lookup"><span data-stu-id="7271e-238">The state or province in the user's address.</span></span>|
|<span data-ttu-id="7271e-239">streetAddress</span><span class="sxs-lookup"><span data-stu-id="7271e-239">streetAddress</span></span>|<span data-ttu-id="7271e-240">String</span><span class="sxs-lookup"><span data-stu-id="7271e-240">String</span></span>|<span data-ttu-id="7271e-241">ユーザーの勤務先の番地。</span><span class="sxs-lookup"><span data-stu-id="7271e-241">The street address of the user's place of business.</span></span>|
|<span data-ttu-id="7271e-242">surname</span><span class="sxs-lookup"><span data-stu-id="7271e-242">surname</span></span>|<span data-ttu-id="7271e-243">String</span><span class="sxs-lookup"><span data-stu-id="7271e-243">String</span></span>|<span data-ttu-id="7271e-244">ユーザーの姓。</span><span class="sxs-lookup"><span data-stu-id="7271e-244">The user's surname (family name or last name).</span></span>|
|<span data-ttu-id="7271e-245">usageLocation</span><span class="sxs-lookup"><span data-stu-id="7271e-245">usageLocation</span></span>|<span data-ttu-id="7271e-246">String</span><span class="sxs-lookup"><span data-stu-id="7271e-246">String</span></span>|<span data-ttu-id="7271e-247">2 文字の国コード (ISO 規格 3166)</span><span class="sxs-lookup"><span data-stu-id="7271e-247">A two-letter country code (ISO standard 3166).</span></span> <span data-ttu-id="7271e-248">国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。</span><span class="sxs-lookup"><span data-stu-id="7271e-248">Required for users who will be assigned licenses due to a legal requirement to check for availability of services in countries or regions.</span></span>  <span data-ttu-id="7271e-249">たとえば、"US"、"JP"、"GB" などです。</span><span class="sxs-lookup"><span data-stu-id="7271e-249">Examples include: "US", "JP", and "GB".</span></span> <span data-ttu-id="7271e-250">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="7271e-250">Not nullable.</span></span>|
|<span data-ttu-id="7271e-251">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7271e-251">userPrincipalName</span></span>|<span data-ttu-id="7271e-252">String</span><span class="sxs-lookup"><span data-stu-id="7271e-252">String</span></span>|<span data-ttu-id="7271e-p117">ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](../resources/organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7271e-p117">The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](../resources/organization.md). Supports $filter and $orderby.</span></span>
|<span data-ttu-id="7271e-260">userType</span><span class="sxs-lookup"><span data-stu-id="7271e-260">userType</span></span>|<span data-ttu-id="7271e-261">String</span><span class="sxs-lookup"><span data-stu-id="7271e-261">String</span></span>|<span data-ttu-id="7271e-262">ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。</span><span class="sxs-lookup"><span data-stu-id="7271e-262">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”.</span></span>          |

## <a name="response"></a><span data-ttu-id="7271e-263">応答</span><span class="sxs-lookup"><span data-stu-id="7271e-263">Response</span></span>

<span data-ttu-id="7271e-264">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7271e-264">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7271e-265">例</span><span class="sxs-lookup"><span data-stu-id="7271e-265">Example</span></span>

### <a name="example-1-update-properties-of-the-signed-in-user"></a><span data-ttu-id="7271e-266">例 1: サインインしているユーザーのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="7271e-266">Example 1: Update properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="7271e-267">要求</span><span class="sxs-lookup"><span data-stu-id="7271e-267">Request</span></span>

<span data-ttu-id="7271e-268">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7271e-268">The following example shows how to create a request context.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7271e-269">HTTP</span><span class="sxs-lookup"><span data-stu-id="7271e-269">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7271e-270">C#</span><span class="sxs-lookup"><span data-stu-id="7271e-270">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7271e-271">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7271e-271">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7271e-272">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7271e-272">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7271e-273">Java</span><span class="sxs-lookup"><span data-stu-id="7271e-273">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7271e-274">応答</span><span class="sxs-lookup"><span data-stu-id="7271e-274">Response</span></span>
<span data-ttu-id="7271e-275">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7271e-275">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-properties-of-the-specified-user"></a><span data-ttu-id="7271e-276">例 2: 指定したユーザーのプロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="7271e-276">Example 2: Update properties of the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="7271e-277">要求</span><span class="sxs-lookup"><span data-stu-id="7271e-277">Request</span></span>

<span data-ttu-id="7271e-278">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="7271e-278">The following example shows how to create a request context.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7271e-279">HTTP</span><span class="sxs-lookup"><span data-stu-id="7271e-279">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_other_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id}
Content-type: application/json

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "officeLocation": "city-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7271e-280">C#</span><span class="sxs-lookup"><span data-stu-id="7271e-280">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-other-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7271e-281">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7271e-281">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-other-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7271e-282">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7271e-282">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-other-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7271e-283">Java</span><span class="sxs-lookup"><span data-stu-id="7271e-283">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-other-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7271e-284">応答</span><span class="sxs-lookup"><span data-stu-id="7271e-284">Response</span></span>

<span data-ttu-id="7271e-285">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7271e-285">The following example shows the response.</span></span>
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
