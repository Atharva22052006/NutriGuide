import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';
import 'package:font_awesome_flutter/font_awesome_flutter.dart';

void main() {
  runApp(const NutriGuideApp());
}

class NutriGuideApp extends StatelessWidget {
  const NutriGuideApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'NutriGuide',
      theme: ThemeData(
        primaryColor: const Color(0xFF22C55E),
        textTheme: GoogleFonts.poppinsTextTheme(),
      ),
      home: const LoginPage(),
      debugShowCheckedModeBanner: false,
    );
  }
}

class LoginPage extends StatefulWidget {
  const LoginPage({super.key});

  @override
  State<LoginPage> createState() => _LoginPageState();
}

class _LoginPageState extends State<LoginPage> {
  bool _isButtonHovered = false;

  @override
  Widget build(BuildContext context) {
    final screenWidth = MediaQuery.of(context).size.width;
    final isSmallScreen = screenWidth < 640;

    return Scaffold(
      backgroundColor: const Color(0xFFF3F4F6), // bg-gray-100
      body: SafeArea(
        child: SingleChildScrollView(
          child: Column(
            children: [
              // Navbar
              Container(
                padding: EdgeInsets.symmetric(
                  horizontal: isSmallScreen ? 16 : 24,
                  vertical: 16,
                ),
                decoration: const BoxDecoration(
                  color: Colors.white,
                  boxShadow: [
                    BoxShadow(
                      color: Colors.black12,
                      blurRadius: 8,
                      offset: Offset(0, 2),
                    ),
                  ],
                ),
                child: Row(
                  mainAxisAlignment: MainAxisAlignment.spaceBetween,
                  children: [
                    Text(
                      'NutriGuide',
                      style: GoogleFonts.poppins(
                        fontSize: isSmallScreen ? 20 : 24,
                        fontWeight: FontWeight.bold,
                        color: const Color(0xFF16A34A), // text-green-600
                      ),
                    ),
                    Row(
                      children: [
                        _buildNavItem('Home', isSmallScreen),
                        SizedBox(width: isSmallScreen ? 8 : 16),
                        _buildNavItem('Plans', isSmallScreen),
                        SizedBox(width: isSmallScreen ? 8 : 16),
                        _buildNavItem('Recipes', isSmallScreen),
                        SizedBox(width: isSmallScreen ? 8 : 16),
                        _buildNavItem('Track', isSmallScreen),
                        SizedBox(width: isSmallScreen ? 8 : 16),
                        ElevatedButton(
                          onPressed: () {},
                          style: ElevatedButton.styleFrom(
                            backgroundColor: const Color(0xFF22C55E), // bg-green-500
                            foregroundColor: Colors.white,
                            padding: EdgeInsets.symmetric(
                              horizontal: isSmallScreen ? 12 : 16,
                              vertical: isSmallScreen ? 6 : 8,
                            ),
                            shape: RoundedRectangleBorder(
                              borderRadius: BorderRadius.circular(999),
                            ),
                            textStyle: TextStyle(
                              fontSize: isSmallScreen ? 12 : 14,
                              fontWeight: FontWeight.w600,
                            ),
                          ),
                          child: const Text('Sign Up'),
                        ),
                      ],
                    ),
                  ],
                ),
              ),

              // Login Section
              Container(
                decoration: const BoxDecoration(
                  gradient: LinearGradient(
                    begin: Alignment.topLeft,
                    end: Alignment.bottomRight,
                    colors: [Color(0xFF6EE7B7), Color(0xFF3B82F6)],
                  ),
                ),
                padding: EdgeInsets.symmetric(vertical: isSmallScreen ? 64 : 80),
                child: Center(
                  child: Container(
                    constraints: const BoxConstraints(maxWidth: 448),
                    margin: EdgeInsets.symmetric(horizontal: isSmallScreen ? 16 : 24),
                    padding: EdgeInsets.all(isSmallScreen ? 24 : 32),
                    decoration: BoxDecoration(
                      color: Colors.white,
                      borderRadius: BorderRadius.circular(8),
                      boxShadow: const [
                        BoxShadow(
                          color: Colors.black12,
                          blurRadius: 8,
                          offset: Offset(0, 4),
                        ),
                      ],
                    ),
                    child: Column(
                      children: [
                        Text(
                          'Welcome Back',
                          style: TextStyle(
                            fontSize: isSmallScreen ? 24 : 30,
                            fontWeight: FontWeight.bold,
                            color: const Color(0xFF1F2937), // text-gray-800
                          ),
                        ),
                        const SizedBox(height: 8),
                        Text(
                          'Log in to continue your journey with NutriGuide',
                          style: TextStyle(
                            fontSize: isSmallScreen ? 12 : 14,
                            color: const Color(0xFF4B5563), // text-gray-600
                          ),
                          textAlign: TextAlign.center,
                        ),
                        const SizedBox(height: 24),
                        TextFormField(
                          decoration: InputDecoration(
                            labelText: 'Email',
                            hintText: 'you@example.com',
                            border: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(6),
                            ),
                            focusedBorder: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(6),
                              borderSide: const BorderSide(
                                color: Color(0xFF22C55E),
                                width: 2,
                              ),
                            ),
                            contentPadding: const EdgeInsets.symmetric(
                              horizontal: 12,
                              vertical: 10,
                            ),
                            labelStyle: const TextStyle(
                              color: Color(0xFF374151), // text-gray-700
                            ),
                          ),
                          keyboardType: TextInputType.emailAddress,
                        ),
                        const SizedBox(height: 16),
                        TextFormField(
                          decoration: InputDecoration(
                            labelText: 'Password',
                            hintText: '••••••••',
                            border: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(6),
                            ),
                            focusedBorder: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(6),
                              borderSide: const BorderSide(
                                color: Color(0xFF22C55E),
                                width: 2,
                              ),
                            ),
                            contentPadding: const EdgeInsets.symmetric(
                              horizontal: 12,
                              vertical: 10,
                            ),
                            labelStyle: const TextStyle(
                              color: Color(0xFF374151), // text-gray-700
                            ),
                          ),
                          obscureText: true,
                        ),
                        const SizedBox(height: 12),
                        Align(
                          alignment: Alignment.centerRight,
                          child: TextButton(
                            onPressed: () {},
                            child: Text(
                              'Forgot Password?',
                              style: TextStyle(
                                fontSize: 12,
                                color: const Color(0xFF16A34A), // text-green-600
                              ),
                            ),
                          ),
                        ),
                        const SizedBox(height: 8),
                        GestureDetector(
                          onTap: () {
                            setState(() {
                              _isButtonHovered = !_isButtonHovered;
                            });
                          },
                          child: AnimatedContainer(
                            duration: const Duration(milliseconds: 300),
                            width: double.infinity,
                            height: isSmallScreen ? 40 : 44,
                            decoration: BoxDecoration(
                              color: const Color(0xFF22C55E),
                              borderRadius: BorderRadius.circular(999),
                              boxShadow: const [
                                BoxShadow(
                                  color: Color(0xFF15803D),
                                  blurRadius: 8,
                                  offset: Offset(0, 2),
                                ),
                              ],
                            ),
                            child: Row(
                              mainAxisAlignment: MainAxisAlignment.center,
                              children: [
                                Text(
                                  'Log In',
                                  style: TextStyle(
                                    color: Colors.white,
                                    fontSize: isSmallScreen ? 14 : 16,
                                    fontWeight: FontWeight.w500,
                                  ),
                                ),
                                const SizedBox(width: 8),
                                AnimatedContainer(
                                  duration: const Duration(milliseconds: 300),
                                  width: _isButtonHovered ? 80 : 36,
                                  height: 36,
                                  decoration: BoxDecoration(
                                    color: Colors.white,
                                    borderRadius: BorderRadius.circular(999),
                                    boxShadow: const [
                                      BoxShadow(
                                        color: Color(0xFF15803D),
                                        blurRadius: 4,
                                        offset: Offset(0.1, 0.1),
                                      ),
                                    ],
                                  ),
                                  child: const Center(
                                    child: Icon(
                                      Icons.arrow_forward,
                                      color: Color(0xFF15803D),
                                      size: 20,
                                    ),
                                  ),
                                ),
                              ],
                            ),
                          ),
                        ),
                        const SizedBox(height: 16),
                        Text.rich(
                          TextSpan(
                            text: "Don't have an account? ",
                            style: TextStyle(
                              fontSize: 12,
                              color: const Color(0xFF4B5563), // text-gray-600
                            ),
                            children: [
                              WidgetSpan(
                                child: GestureDetector(
                                  onTap: () {},
                                  child: Text(
                                    'Sign Up',
                                    style: TextStyle(
                                      fontSize: 12,
                                      color: const Color(0xFF16A34A), // text-green-600
                                      fontWeight: FontWeight.w600,
                                    ),
                                  ),
                                ),
                              ),
                            ],
                          ),
                          textAlign: TextAlign.center,
                        ),
                      ],
                    ),
                  ),
                ),
              ),

              // Footer
              Container(
                color: const Color(0xFF1F2937), // bg-gray-800
                padding: EdgeInsets.symmetric(
                  horizontal: isSmallScreen ? 16 : 24,
                  vertical: isSmallScreen ? 32 : 40,
                ),
                child: Column(
                  children: [
                    Row(
                      crossAxisAlignment: CrossAxisAlignment.start,
                      children: [
                        // Quick Links
                        Expanded(
                          child: Column(
                            crossAxisAlignment: CrossAxisAlignment.start,
                            children: [
                              Text(
                                'Quick Links',
                                style: TextStyle(
                                  fontSize: 18,
                                  fontWeight: FontWeight.w600,
                                  color: Colors.white,
                                ),
                              ),
                              const SizedBox(height: 8),
                              _buildFooterLink('About Us', isSmallScreen),
                              _buildFooterLink('Contact', isSmallScreen),
                              _buildFooterLink('Privacy Policy', isSmallScreen),
                            ],
                          ),
                        ),
                        // Quick Health Tip
                        Expanded(
                          child: Column(
                            children: [
                              Text(
                                'Quick Health Tip',
                                style: TextStyle(
                                  fontSize: 18,
                                  fontWeight: FontWeight.w600,
                                  color: Colors.white,
                                ),
                              ),
                              const SizedBox(height: 16),
                              Container(
                                padding: EdgeInsets.all(isSmallScreen ? 12 : 16),
                                decoration: BoxDecoration(
                                  gradient: const LinearGradient(
                                    begin: Alignment.topRight,
                                    end: Alignment.bottomLeft,
                                    colors: [Color(0xFF1F2937), Color(0xFF374151)],
                                  ),
                                  border: Border.all(color: const Color(0xFF4B5563)),
                                  borderRadius: BorderRadius.circular(12),
                                  boxShadow: const [
                                    BoxShadow(
                                      color: Colors.black12,
                                      blurRadius: 6,
                                      offset: Offset(0, 4),
                                    ),
                                  ],
                                ),
                                child: Column(
                                  crossAxisAlignment: CrossAxisAlignment.start,
                                  children: [
                                    Text(
                                      'Stay Hydrated',
                                      style: TextStyle(
                                        fontSize: isSmallScreen ? 12 : 14,
                                        fontWeight: FontWeight.w600,
                                        color: const Color(0xFF22C55E),
                                      ),
                                    ),
                                    const SizedBox(height: 8),
                                    Text(
                                      'Drinking enough water daily boosts energy, improves digestion, and keeps your skin glowing.',
                                      style: TextStyle(
                                        fontSize: isSmallScreen ? 11 : 12,
                                        color: const Color(0xFF9CA3AF),
                                      ),
                                    ),
                                  ],
                                ),
                              ),
                            ],
                          ),
                        ),
                        // Follow Us
                        Expanded(
                          child: Column(
                            crossAxisAlignment: CrossAxisAlignment.start,
                            children: [
                              Text(
                                'Follow Us',
                                style: TextStyle(
                                  fontSize: 18,
                                  fontWeight: FontWeight.w600,
                                  color: Colors.white,
                                ),
                              ),
                              const SizedBox(height: 8),
                              Row(
                                mainAxisAlignment: MainAxisAlignment.start,
                                children: [
                                  _buildSocialIcon(
                                    icon: FontAwesomeIcons.facebookF,
                                    tooltip: 'Facebook',
                                    activeColor: const Color(0xFF1877F2),
                                    isSmallScreen: isSmallScreen,
                                  ),
                                  const SizedBox(width: 8),
                                  _buildSocialIcon(
                                    icon: FontAwesomeIcons.twitter,
                                    tooltip: 'Twitter',
                                    activeColor: const Color(0xFF1DA1F2),
                                    isSmallScreen: isSmallScreen,
                                  ),
                                  const SizedBox(width: 8),
                                  _buildSocialIcon(
                                    icon: FontAwesomeIcons.instagram,
                                    tooltip: 'Instagram',
                                    activeColor: const Color(0xFFE4405F),
                                    isSmallScreen: isSmallScreen,
                                  ),
                                ],
                              ),
                            ],
                          ),
                        ),
                      ],
                    ),
                    const SizedBox(height: 24),
                    Text(
                      '© 2025 NutriGuide. All rights reserved.',
                      style: TextStyle(
                        fontSize: isSmallScreen ? 12 : 14,
                        color: const Color(0xFF9CA3AF), // text-gray-400
                      ),
                      textAlign: TextAlign.center,
                    ),
                  ],
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }

  Widget _buildNavItem(String title, bool isSmallScreen) {
    return GestureDetector(
      onTap: () {},
      child: Text(
        title,
        style: TextStyle(
          fontSize: isSmallScreen ? 12 : 14,
          color: const Color(0xFF4B5563), // text-gray-600
          fontWeight: FontWeight.w500,
        ),
      ),
    );
  }

  Widget _buildFooterLink(String title, bool isSmallScreen) {
    return Padding(
      padding: const EdgeInsets.only(bottom: 8),
      child: GestureDetector(
        onTap: () {},
        child: Text(
          title,
          style: TextStyle(
            fontSize: isSmallScreen ? 12 : 14,
            color: const Color(0xFF9CA3AF), // text-gray-400
          ),
        ),
      ),
    );
  }

  Widget _buildSocialIcon({
    required IconData icon,
    required String tooltip,
    required Color activeColor,
    required bool isSmallScreen,
  }) {
    return StatefulBuilder(
      builder: (context, setState) {
        bool isHovered = false;
        return GestureDetector(
          onTap: () {
            setState(() {
              isHovered = !isHovered;
            });
          },
          child: Stack(
            alignment: Alignment.center,
            children: [
              Container(
                width: 36,
                height: 36,
                decoration: BoxDecoration(
                  color: Colors.white,
                  shape: BoxShape.circle,
                  boxShadow: const [
                    BoxShadow(
                      color: Colors.black26,
                      blurRadius: 5,
                      offset: Offset(0, 2),
                    ),
                  ],
                ),
                child: Icon(
                  icon,
                  size: 16,
                  color: isHovered ? activeColor : Colors.black,
                ),
              ),
              AnimatedPositioned(
                duration: const Duration(milliseconds: 200),
                top: isHovered ? -35 : -20,
                curve: Curves.easeInOut,
                child: AnimatedOpacity(
                  opacity: isHovered ? 1.0 : 0.0,
                  duration: const Duration(milliseconds: 200),
                  child: Container(
                    padding: const EdgeInsets.symmetric(horizontal: 6, vertical: 4),
                    decoration: BoxDecoration(
                      color: const Color(0xFF22C55E),
                      borderRadius: BorderRadius.circular(4),
                      boxShadow: const [
                        BoxShadow(
                          color: Colors.black26,
                          blurRadius: 5,
                          offset: Offset(0, 2),
                        ),
                      ],
                    ),
                    child: Text(
                      tooltip,
                      style: const TextStyle(
                        fontSize: 12,
                        color: Colors.white,
                        fontWeight: FontWeight.w500,
                      ),
                    ),
                  ),
                ),
              ),
              if (isHovered)
                Positioned(
                  top: -8,
                  child: Transform.rotate(
                    angle: 45 * 3.14159 / 180,
                    child: Container(
                      width: 6,
                      height: 6,
                      color: const Color(0xFF22C55E),
                    ),
                  ),
                ),
            ],
          ),
        );
      },
    );
  }
}